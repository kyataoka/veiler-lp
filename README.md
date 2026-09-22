# Veiler — 公開サイト

[Veiler](https://apps.apple.com/jp/app/id6790334654) の紹介ページと、
プライバシーポリシー・利用規約。GitHub Pages で
**<https://veiler.kyatatata.com>** に公開しています。

*The public website for Veiler, an iOS app that keeps photos and videos in a
passcode-locked vault. Japanese is the authoritative text; the English pages
are translations of it.*

|  | 日本語 | English |
| --- | --- | --- |
| 紹介ページ | [/](https://veiler.kyatatata.com/) | [/en/](https://veiler.kyatatata.com/en/) |
| プライバシーポリシー | [/privacy/ja/](https://veiler.kyatatata.com/privacy/ja/) | [/privacy/en/](https://veiler.kyatatata.com/privacy/en/) |
| 利用規約 | [/terms/ja/](https://veiler.kyatatata.com/terms/ja/) | [/terms/en/](https://veiler.kyatatata.com/terms/en/) |

## 文書の扱い

- **日本語が正文**です。英語は訳であり、食い違いがある場合は日本語が優先する旨を
  各文書の冒頭に記しています。日本語を改めたときは英語も同時に改めます
- 文書の出どころはこのリポジトリだけに置き、別の場所に写しを作りません
- 法務文書には**現に提供している機能**を記します。予定や検討中の内容は含めません
- 紹介ページで挙げる機能も、提供済みのものに限ります

## URL は変更しません

`privacy` と `terms` の4つの URL は、配布済みのアプリから直接開かれます
（設定画面の「プライバシーポリシー」「利用規約」、および初回起動時の同意画面）。
プライバシーポリシーの URL は App Store Connect にも登録しています。

そのためパスを変更すると、すでにお使いの版から文書を開けなくなります。各文書の
permalink をファイルパスから導出せず固定しているのは、この理由によります。

同じ理由から、サイトのアドレスはリポジトリ名から独立させています。GitHub は
リポジトリ名を変更したとき、プロジェクトサイトの URL だけリダイレクトしないため
（[Renaming a repository][rn]）、独自ドメインを割り当てています。

[rn]: https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository

## 規約を改めるとき

利用規約の**最終改定日**を変更したときは、アプリが同意を記録する際の版の値も
同じものに合わせます。アプリは初回起動時の同意でこの値を端末に保存するため、
食い違うと同意された版を特定できなくなります。

## 構成

| パス | 内容 |
| --- | --- |
| `index.html`, `en/index.html` | 紹介ページ。レイアウトは `_layouts/landing.html` |
| `privacy/*.md`, `terms/*.md` | 法務文書。レイアウトは `_layouts/document.html` |
| `assets/` | アイコン、App Store バッジ、スクリーンショット |

紹介ページのテーマは3つの状態を持ちます — OS の設定に従う既定、明示的なライト、
明示的なダーク。CSS 変数は素の `:root` に完全な組を定義し、
`prefers-color-scheme` と `[data-theme]` では上書きのみを行います。
スクリーンショットの明暗も CSS で切り替えます。`<picture>` の
`media="(prefers-color-scheme: dark)"` は OS の設定にしか反応せず、ページ上の
切り替えボタンを操作したときに画像だけが元のままになるためです。

## ローカルビルド

用意していません。Gemfile を置いていないため、確認は push して GitHub Pages の
ビルドを待つ形になります（おおむね 30〜60 秒）。

## ライセンス

本リポジトリの文書および紹介ページの内容は Veiler の法務文書・製品情報であり、
再配布や転載を目的としたものではありません。
