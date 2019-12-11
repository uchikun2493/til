
# fish

bashに不満が出てきたので高速と名高いfishを試す会

## 導入
```
$ # インストール
$ sudo apt terminator fish
$ # 確認作業
$ # "/usr/bin/fish"が表示されてなければ"which fish"`の結果を"/etc/shells"に追記する  
$ grep fish /etc/shells  
$ # デフォルトのshellを変更する
$ chsh -s /usr/bin/fish  
```

## カスタマイズ

```
$ # ブラウザ上である程度は設定を変更できる
$ fish_config
```

```
$ # aliasやpathのの編集
$ vim ~/.config/fish/config.fish
```


## cudaやcudnnのパスを通す


~/.config/fish/config.fishに追記
```
set PATH /usr/local/cuda/bin $PATH
set PATH /usr/local/cuda/lib64 $PATH
```

## pyenvのpathを通す

~/.config/fish/config.fishに追記
```
set PATH $HOME/.pyenv/shims $PATH
eval (pyenv init - | source)
```
## aliasの設定

~/.config/fish/config.fishに追記
```
# ex: :qでexit
alias q='exit'
```

