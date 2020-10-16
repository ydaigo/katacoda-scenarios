# Docker初歩

## 自己紹介
- 山本大悟
- 富山県でSier
- 最近ボルダリングにはまっている

## このLTの対象
- Dockerの基礎的な内容を知りたい人
- Dockerという言葉を聞いたことがあり概要を知りたい人

## このLTの流れ
1. はじめに
2. Dockerの仕組み
3. コマンドの詳しい説明
4. Docker Compose
5. 機械学習の環境を作成する
# はじめに
## Katacodaとは？
- オライリーが作成したソフトウェアの学習プラットフォームである。
- ブラウザでLinuxのコマンドやサーバーソフトvs-codeが使える
- 手軽に使えて学習コンテンツを共有するのに最適
- Dockerやkubernetなどの公式の学習コンテンツがある。
- この教材の環境はUbuntu 20.04がベースとなっています。  
  下記のコマンドでバージョンを確認  
`lsb_release -a`{{execute T1}}
## Dockerとは？
コンテナ型の仮想環境を作成、配布、実行するためのプラットフォームだ。  
まずは、実際に動かしてみよう。*1
1. dockerがインストールされていることを確認する。  
`docker -v`{{execute T1}}
2. dockerを使ってWebサーバを立ち上げる。  
`docker run --name test -p 80:80 -d nginx`{{execute T1}}  
このように簡単にサーバーを立ち上げることができる。

## Dockerを使うと何がうれしい？*2
- 開発環境や本番環境を配布しやすい。
- アプリケーションの開発から本番運用までの期間が短くなる。



## 参考
*1 https://docs.nginx.com/nginx/admin-guide/installing-nginx/installing-nginx-docker/
*2 https://docs.docker.com/get-started/overview/