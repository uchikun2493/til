# dein.vim

## 遅延読み込みの設定を行う

```

" Required:
if dein#load_state('~/.cache/dein')
    call dein#begin('~/.cache/dein')

    " プラグインリストを収めた TOML ファイル
    " ~/.vim/rc/dein.toml,deinlazy.tomlを用意する
    " let g:rc_dir    = expand('~/.vim/toml')
    " let s:toml      = g:rc_dir . '/dein.toml'
    " let s:lazy_toml = g:rc_dir . '/dein_lazy.toml'

    " TOML を読み込み、キャッシュしておく
    " call dein#load_toml(s:toml,      {'lazy': 0})
    " call dein#load_toml(s:lazy_toml, {'lazy': 1})

    " Required:
    call dein#end()
    call dein#save_state()
endif

```

