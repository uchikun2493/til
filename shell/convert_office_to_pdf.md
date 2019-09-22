# OfficeをPDFに変換する

## LibrerOfficeをインストール

```
$ brew cask install libreoffice-language-pack
```

参考

[Homebrew-CaskでLibreOfficeの日本語版をインストール](https://blog.n-z.jp/blog/2018-01-23-homebrew-libreoffice.html)

## 変換

```
/Applications/LibreOffice.app/Contents/MacOS/soffice --headless --nologo --nofirststartwizard --convert-to pdf --outdir 出力先のディレクトリ ファイルパス
```

上記をaliasに登録しておくと便利

