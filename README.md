# alexa-hosted-sample-python-chatgpt

ChatGPT APIを使ってAIと自由な会話を行うAlexaスキルのサンプルです。Alexa-hostedでインポートして使えます。

- ChatGPT APIを使用　※OPEN AIのAPIキーが必要です
- ダイアログモデルを使用してユーザの自由な発話を受け取り
- セッションアトリビュートで会話のコンテキストを保持

## 使い方

1. Alexa開発者コンソールで新規スキル作成
  - 適当なスキル名を設定（呼び出し名になります）
  - カスタム・Alexa-Hosted(Python)を選択
  - 「スキルを作成」をクリック
2. テンプレートの選択画面で「スキルをインポート」をクリックして、URLに `https://github.com/kun432/alexa-hosted-sample-python-chatgpt.git` を入力してインポート
3. コードエディタを開いて`lambda/dot-env`を`lambda/.env`にリネームしてOpenAIのAPIキーをセット。保存・デプロイ
4. テストシミュレータで「開発中」ステージに変更
5. 呼び出し名で起動。


## ToDo

- 保持する会話コンテキストには上限を設けていない。ChatGPT APIのリクエストサイズを踏まえた何らかの処理を追加する。
- プロンプトは見直しの余地がある。
