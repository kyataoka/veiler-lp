# Veiler の公開サイト

Veiler の紹介ページと、プライバシーポリシー・利用規約。**ここが唯一の原本**で、
GitHub Pages がそのまま公開している。

|  | 日本語 | English |
| --- | --- | --- |
| 紹介ページ | [/](https://veiler.kyatatata.com/) | [/en/](https://veiler.kyatatata.com/en/) |
| プライバシーポリシー | [/privacy/ja/](https://veiler.kyatatata.com/privacy/ja/) | [/privacy/en/](https://veiler.kyatatata.com/privacy/en/) |
| 利用規約 | [/terms/ja/](https://veiler.kyatatata.com/terms/ja/) | [/terms/en/](https://veiler.kyatatata.com/terms/en/) |

## URL は動かせない

`privacy` と `terms` の4つの URL は、**すでに配布したアプリのバイナリに直接
書かれている**（`lib/core/legal_urls.dart`）。設定画面の「プライバシーポリシー」
「利用規約」と、初回起動時の同意画面がここを開く。プライバシーポリシーは
App Store Connect にも登録してある。

だからパスを変えると、手元にある版からは開けなくなり、アプリを出し直すまで
直せない。各文書の permalink をファイルパスから導出せず固定してあるのはこのため。

同じ理由で、**リポジトリ名を変えるとサイトの URL は壊れる**。GitHub はリネーム時、
プロジェクトサイトの URL だけリダイレクトしない（[Renaming a repository][rn]）。
名前を変えるなら、先に独自ドメインを設定して URL をリポジトリ名から切り離すこと。

[rn]: https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository

## 日本語が原本

英語は便宜的な訳。食い違ったときは日本語が優先すると各文書の冒頭に書いてある。
日本語を直したら英語も直すこと — 訳が古いのは、訳が無いより悪い。

以前は Google Sites に手で貼っていた。掲載物とリポジトリが3回ズレて、そのうち
1回は「広告 SDK を一切組み込んでいません」と書いたまま広告付きで出しかけた。
コピーを2つ持たないのがその修正である。

## 変更するときに合わせるもの

利用規約の **最終改定日** を変えたら、アプリ側の `kTermsVersion`
（`lib/core/legal_urls.dart`）も同じ値にする。アプリは初回起動時の同意でこの値を
端末に記録するため、食い違うと「何に同意したか」が答えられなくなる。

紹介ページで機能を挙げるときは、アプリ側の `lib/core/features.dart` を確認する。
実装もテストもあるが導線だけ隠してある機能があり（書類・スライドショー・検索）、
それを載せると存在しない機能の宣伝になる。一度やって直した。

法務文書は**今出荷しているもの**を説明する。将来の予定に合わせて表現をぼかすと、
事実と文書がずれる。紹介ページ側で「など」と書くのはよいが、規約とポリシーでは
書かない。

## 構成

| パス | 中身 |
| --- | --- |
| `index.html`, `en/index.html` | 紹介ページ。レイアウトは `_layouts/landing.html` |
| `privacy/*.md`, `terms/*.md` | 法務文書。レイアウトは `_layouts/document.html` |
| `assets/` | アイコン、App Store バッジ（JP/US）、スクリーンショット |

紹介ページのテーマは3状態ある — OS 設定に従う既定、明示的なライト、明示的な
ダーク。CSS の変数は素の `:root` に完全な組を置き、`prefers-color-scheme` と
`[data-theme]` では上書きだけをする。スクリーンショットの明暗の出し分けも CSS
で行う。`<picture>` の `media="(prefers-color-scheme: dark)"` は OS 設定にしか
反応せず、ヘッダーの切り替えボタンを押したときに画像だけが取り残されるため。

## ローカルビルド

用意していない。Gemfile を置いていないので、確認は push して GitHub Pages の
ビルドを待つ形になる。反映はおおむね 30〜60 秒。
