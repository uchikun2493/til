
# Shell Tips

## 違うShellを立ち上げてファイルを実行したい

直接実行するならこんな感じ，終了すると自動的にターミナルを閉じます
```
gnome-terminal -- ~/path_1/hoge
```

複数のコマンドを続けて実行して欲しい，exitを入れると終了で自動に閉じてくれる
```
gnome-terminal -- bash -c "cd ~/catkin_ws/src/consai2; roslaunch consai2_examples mft_atk.launch; exit; bash"
```
