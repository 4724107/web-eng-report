# 第3回 Webエンジニアリング演習 レポート
## 学籍番号
4724107
## イメージとコンテナの違い
（自分の言葉で説明）
Dockerイメージはアプリの実行に必要なコードや環境をまとめた読み取り専用のパッケージで、Dockerコンテナはそのイメージを基に作られた実際に動かす環境のことをいう。同じイメージから複数のコンテナを起動でき、コンテナを削除しても元のイメージは残る。


## Dockerfileの各行の役割
（FROMとCOPYを説明）
FROMは、土台となるベースのイメージを指定する命令。
COPYは、ホスト側のファイルをDockerイメージ内へコピーする命令。

## 動作確認
（変更後の見出しとdocker compose psの結果）
変更後の見出し：Docker Composeで配信中
docker compose psの結果：
NAME                   IMAGE                COMMAND                  SERVICE   CREATED          STATUS          PORTS
web-eng-docker-web-1   web-eng-docker-web   "/docker-entrypoint.…"   web       25 seconds ago   Up 24 seconds   0.0.0.0:8080->80/tcp, [::]:8080->80/tcp