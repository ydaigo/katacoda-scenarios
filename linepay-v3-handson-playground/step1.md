### 1-1. Docker初歩

# 自己紹介
- 山本大悟
- 富山県でSier
- 最近ボルダリングにはまっている

# 目次

# Dockerとは？
コンテナ型の仮想環境を作成、配布、実行するためのプラットフォームだ。  
まずは、実際に動かしてみよう。*1
1. dockerがインストールされていることを確認する。  
`docker -v`{{execute T1}}
2. dockerを使ってWebサーバを立ち上げる。
`docker run -p 80:80 -d nginx`{{execute T1}}


# 参考
*1 https://docs.nginx.com/nginx/admin-guide/installing-nginx/installing-nginx-docker/