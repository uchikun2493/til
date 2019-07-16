# リポジトリ名をあとから変更する

## GitHub側の操作
"対象リポジトリ -> Setting -> Rename"で変更

ex.
```
repo_old -> repo_new に変更したとする
```

## ローカル側の操作
対象ディレクトリ -> .git > config

```
[remote "origin"]
    url = https://github.com/hoge/repo_old.git
    fetch = +refs/heads/*:refs/remotes/origin/*
```

```
[remote "origin"]
    url = https://github.com/hoge/repo_new.git
    fetch = +refs/heads/*:refs/remotes/origin/*
```
