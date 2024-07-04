# 1行でLEMP環境構築

サーバに`root`ログインし１行のコマンドを実行するだけでDockerコンテナのLEMP環境が構築できるスクリプトです。

## 対象OS

- Ubuntu 22
- Ubuntu 20

## ライセンス

[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)

# 内容

Ansibleのローカル実行でDocker環境をインストールし、DockerコンテナでLEMP環境を構築します。

## LEMP環境

- Nginx(Dockerコンテナ) - Nginx最新
- PHP(Dockerコンテナ) - PHP8最新
- db(Dockerコンテナ) - Mariadb最新

## インストールモジュール

- docker v27

# 使い方

新規にOSをインストールしたサーバに`root`でログインし、以下の１行のコマンドをそのままコピーして実行します。

## 実行コマンド

```
curl https://raw.githubusercontent.com/czbone/oneliner-lemp/master/script/start.sh | bash
```

## テスト

以下のURLにアクセスし、エラーなしで画面が表示されればOKです。

- http://[IPアドレス]/_sample/index.php
- http://[IPアドレス]/_sample/index2.php
