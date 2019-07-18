cd ~/.ssh

※GitHubに登録しているEmailアドレスを使うのが一般的のようです。

```
$ ssh-keygen -t rsa -C "your_email@example.com"
$ ssh-add ~/.ssh/id_rsa
$ cat /.ssh/id_rsa.pub
```

![](https://qiita.com/suthio/items/2760e4cff0e185fe2db9)
![](http://monsat.hatenablog.com/entry/generating-ssh-keys-for-github)
