# Doker
## Docker とは
- アプリを動かす環境を「箱（コンテナ）」にまとめる技術。
- どこでも同じ環境で動かせる。
- 本番と開発の差が減るのが嬉しい。
## Docker + ローカル環境構築について学んだこと
-Docker の make build は、アプリ動作用のイメージ（環境）を構築するコマンドであることを理解した
-make up を実行することで、Rails API（tech-master）や Frontend（arizona）がコンテナとして起動し、ローカルでアクセスできるようになる仕組みを学んだ
-外部参加者用に 別の DB コンテナ（tech-camp-db） を立ち上げる必要があり、その際 docker-compose.tech-camp.yml を使うことを理解した
-docker ps でコンテナの状態（Running / Healthy）を確認できることを学んだ
