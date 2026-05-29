# Web-android-emulator
Webブラウザから本物のAndroid OSを操作するためのプロジェクトです。

## 🏗️ 全体構成（システム設計）

1. **バックエンド (Android OS本体)**
   - Dockerコンテナ上で動作する本物のAndroid OS「**redroid**」を使用します。
   - サーバー（Linux VPS等）側で起動し、外部からの接続（adb）を待ち受けます。

2. **フロントエンド兼中継サーバー (Webブラウザ表示)**
   - Androidの画面をWebブラウザへ低遅延配信する「**ws-scrcpy**」を使用します。
   - ブラウザ上のクリックやキーボード操作をAndroidに送信します。

## 🚀 構築のステップ

- [ ] 1. Android OS（redroid）を動かすためのLinuxサーバー（VPSなど）を用意する
- [ ] 2. サーバーにDockerをインストールし、redroidイメージを起動する
- [ ] 3. このリポジトリに `ws-scrcpy` のソースコードを取り込み、Web配信UIを構築する
- [ ] 4. WebブラウザからサーバーのAndroid OSに接続し、動作確認を行う
