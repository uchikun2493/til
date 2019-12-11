
## cdの時にlsする

- 関数を追加して，aliasに登録しておくとcdでlsしてくれる
- この例の場合だとlaを実行
- \が重要らしい

```
# aliasの追加
# cでclear 
alias c='clear'

# cdしたらla
function cd_ls() {
  # cdがaliasでループするので\をつける
  \cd "$@" && la
}
alias cd='cd_ls'
```

## clear
```
# clearコマンドを省略
alias c='clear'
```

