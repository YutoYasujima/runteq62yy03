## 初期設定
- 下記のコマンドを実行
  ```
  bundle install
  yarn install
  ```
## デプロイ前
- `master.key`を作り直す必要がある。
- `config/credentials.yml.enc`を削除する。
- 下記のコマンドを実行することで、`master.key`を作れる。
既に存在していればそれが使われる。
また、`credentials.yml.enc`が作り直される。
  ```
  EDITOR=vim rails credentials:edit
  ```
