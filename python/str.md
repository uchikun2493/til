# pythonにおける文字列操作

## パスの作成

```
path1 = './dir'
path2 = 'test.txt'
path = os.path.join(path1, path2)
# ./dir/test.txt
```

## 文字列の結合

- '区切り文字列'.join(連結対象の文字列リスト)

```
a = ['test', 'da', 'yo!']

print(''.join(a))
# testdayo!

print(','.join(a))
# test,da,yo!

print('-'.join(a))
# test-da-yo!


print('\n'.join(a))
# test
# da
# yo!
```


