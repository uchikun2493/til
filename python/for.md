# forループ

```
# リストの例
data = ['d1', 'd2', 'd3']
test = ['t1', 't2', 't3']

# 指定回数ループを回す
for i in range(3):
    print(i, data[i])

# リストのサイズからインデクスを作成
for i in range(len(data)):
    print(i, data[i])

# リストから順番にデータを取り出し
for d in data:
    print(d)

# リストから順番にデータを取り出し、インデックスも取得
for i, d in enumerate(data):
    print(i, d)

# 複数のリストから順番にデータを取り出す
for (d, t) in zip(data, test):
    print(d, t)

# 複数のリストから順番にデータを取り出し、インデックスも取得
for i, (d, t) in enumerate(zip(data, test)):
    print(i, d, t)
```
