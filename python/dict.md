# 辞書型


## dict型のforループ処理

[Pythonの辞書（dict）のforループ処理（keys, values, items）](https://note.nkmk.me/python-dict-keys-values-items/)

- 例では以下のdict型のデータを使う
```
d = {'key1': 1, 'key2': 2, 'key3': 3}
```

```
for k in d:
    print(k)
# key1
# key2
# key3
```

- 応用：複数のディレクトリを作成する

```
dir_save = {'fig':'../output/fig',\
            'data':'../output/data'}
for key in dir_save:
    os.makedirs(dir_save[key], exist_ok = True)

```


