
# vim_tips

vimでヤンクした文字列をクリップボードに共有する

[vimでクリップボード連携を有効にした話](https://pocke.hatenablog.com/entry/2014/10/26/145646)

## vimのxの動作でヤンクレジスタに入らないようにする

```
" xの動作
nnoremap x "_x

" ヤンクレジスタに格納されるコマンド
let g:yankring_n_keys = 'Y D'
" default
" let g:yankring_n_keys = 'Y D x X'
```

