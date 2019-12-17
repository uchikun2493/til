# 補完系の設定メモ

## Shougo/deoplete.nvim

入力の補完に闇の力を与えるものだが，エラーが出て使えなかった

もし，pyenvなどでpythonを設定している場合システムのバージョンと異なることがある

ubuntuの場合はまずシステム側のpythonでpipが使えるようにしておく
```
$ sudo apt install python-pip python-pip3
```

以下を実行，おそらくmacでもubuntuでも大丈夫
```
$ /usr/bin/python3 -m pip install --user pynvim
```

ちなみに以下のコマンドでvimがどのpyhtonを使っているか確認できるらしい
```
:pythonx print(sys.version); print(sys.path)
```
```
```
