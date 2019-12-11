# matplotlib


## フォントを指定する

以下のようにすれば使える

もしエラーが出るようならフォントがダウンロードされていない
```
import matplotlib.pyplot as plt
plt.rcParams['font.family'] = 'Times New Roman'
```

## ubuntuでTimes New Romanが使えない

ubuntuにおいて上記のフォントを指定するでTimes New Romanを指定するとエラーが出る

```
findfont: Font family ['Times New Roman'] not found. Falling back to DejaVu Sans.
```

フォントをダウンロードして~/.cacheを削除する

```
$ sudo apt install msttcorefonts -qq
$ rm ~/.cache/matplotlib -rf
```

