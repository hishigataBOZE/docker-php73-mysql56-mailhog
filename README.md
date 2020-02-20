# Apache＋php7＋MailhogのDocker環境

## インストール要件

- Git
- Docker(docker-composeコマンドが使えること)

1. docker起動

```bash
# ビルドのみ
$ docker-compose build

# ビルドとコンテナの起動
$ docker-compose up -d

# コンテナの停止・削除
$ docker-compose down
```

2. webサイトの表示確認（phpinfo）

    1. `_test/phpinfo.php`を`app/`にコピー（確認後、適宜コピーしたファイルを削除してください）。

    2. 下記にアクセス:
http://localhost:8080/phpinfo.php

3. メール送信の確認

    1. `_test/test_mail.php`を`app/`にコピー（確認後、適宜コピーしたファイルを削除してください）。

    2. 下記にアクセス (Webページからメール送信): 
http://localhost:8080/test_mail.php

    3. 下記にアクセス (メール受信用ページ確認): 
http://localhost:8025/

4. phpMyAdminへのアクセス

http://localhost:8306/
