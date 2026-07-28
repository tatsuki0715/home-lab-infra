## 課題4-3 PHPからMySQLへ接続する３層構成

### 実施内容

VM1(Web1サーバ）
- Apache2+PHPをインストール
- PHP(MySQLi)でMySQLへ接続
- ブラウザからも接続確認

VM2(DBサーバ)

- MySQLをインストール
- homelabデータベースを作成
- appuserを作成
- リモート接続を許可
- bind-address = 0.0.0.0へ変更

### トラブルシューティング

No route to host というエラーが発生

確認した項目
- PHP設定
- Apache設定
- MySQLユーザ権限
- bind-address
- ポート3306待ち受け
- UFW
- iptable
- ping 
- nc
- ip route
- ip neigh

最終的に
sudo ip neigh flush all　
を実行し、ARPキャッシュを再生成することで通信が復旧した

### 学んだこと

- PHPからMySQLへ接続する方法
- WebサーバとDBサーバを分離した構成
- MySQLのリモート接続設定
- Linuxネットワークの基本的な切り分け
- ARPキャッシュが通信へ影響すること
