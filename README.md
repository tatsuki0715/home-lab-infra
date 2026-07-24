
# home-lab-infra

## 2026/07/19

Ubuntu Server構築

・ユーザー追加
・Apacheインストール
・VitualHost作成

# Home Lab Infra

## 構成

- VM1 Web (nginx)
- VM2 DB (MySQL)
- VM3 Test

## 目的
インフラエンジニアとしての基礎力を身につける


## 2026/07/23

### Apache

- DocumentRoot作成
- index.html配置
- Apache設定確認
- Webページ公開


## 202607/23

## 課題3:Apacheログ調査

### 学んだこと
- access.logはアクセス履歴を確認するためのログ
- error.logはApacheのエラーを確認するためのログ
- tail -fでリアルタイム監視ができる
- curlで簡単に動作確認ができる

### 使用したコマンド
- tail -f
- curl
- ls -l


##  課題4-1:MySQLサーバー構築

### 学んだこと
- MySQLをインストールした
- サービスの起動状態を確認した
- データベースを作成した
- テーブルを作成した
- データを登録・確認した

### 使用コマンド
- apt update
- apt install mysql-server
- systemctl status
- systemctl enable
- mysql
- CREATE DATABASE 
- CREATE TABLE
- INSERT
- SELECT

