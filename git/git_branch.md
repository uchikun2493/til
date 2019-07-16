# ブランチを切る

- 現在のブランチから派生ブランチを作成する
```
$ git branch BN
```

- 作業ブランチを変更する
```
$ git checkout BN
```

- 上記２つを一度に行う
```
git checkout -b BN
```

- ローカルブランチを確認する
```
git branch
```

- リモートブランチを確認する
```
git branch -r

```

- 上記２つを一度に行う
```
git branch -a
```

- 現在の作業ブランチに指定ブランチをマージする
```
git merge BN
```

- マージ後でも、元に戻せるようにする
```
git merge --no-ff BN
```

- ブランチの削除
```
git branch -d BN
```

- ブランチの削除(強制的)
```
git branch -D BN
```

- リモート・リポジトリにブランチをプッシュする
```
git push origin BN
```

- リモートブランチからローカルブランチを作成する
```
git checkout -b BN origin/BN
```

- リモートリポジトリのブランチを取得して、ローカルブランチとする
```
git fetch origin RemoteBN:LocalBN
```

- リモートブランチを削除する
```
git push origin :BN
```

- ブランチの派生元ブランチを変更する
```
git rebase BN
```

- ブランチを比較する
```
git diff BN1 BN2
```

