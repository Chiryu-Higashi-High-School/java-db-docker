
## 参考
- https://qiita.com/A-Kira/items/0dda255e00771f556e2a

---
## コマンド

```bash
docker-compose build
```
imageを作成する。
    
```bash
docker-compose up
```
upコマンドでは、キャッシュがある場合はそれを使って一発でイメージの構築から、コンテナの構築・起動までします。

キャッシュがない場合は --build オプションをつけることで、イメージの構築から、コンテナの構築・起動までしてくれます。（ただし、 build コマンドと同じでDockerfileを更新してても反映されません。）

```bash
docker-compose exec web /bin/bash
```
サービスのコンテナ内でコマンドを実行するならexecコマンドも便利です。
docker execコマンドと同じで起動中のコンテナのシェルへ接続することができる

ex:version確認
```bash
docker-compose exec java java --version
```


