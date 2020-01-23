# fishの導入手順

### fish shell のインストール

```
$ brew install fish
```

### ログインシェルの設定変更

```
$ sudo vi /etc/shells
```

```shell:/etc/shells
...
#最後の行に以下を追加
/usr/local/bin/fish
```

```
$ chsh -s /usr/local/bin/fish
```

### 設定ファイルのコピー
```
$ git clone https://github.com/fish-config
$ mv fish-config/.config ~/
$ rm -rf fish-config
```

### powerline/fontsのインストール

```
$ git clone https://github.com/powerline/fonts.git
$ cd fonts
$ ./install.sh
$ cd ../
$ rm -rf fonts
```
