# html5-basic-template-taskrunner

※このタスクランナーはmacでの使用を想定しています（win動作未確認）

## 使い方

1. html5-basic-templateをダウンロード  
ファイルをダウンロードしてきてください

2. Node.jsのインストール  
versionは8系の最新を使ってください  
`.node-version`が入っているので`ndenv`を使用している人は`v8.11.1`が適用されます

3. yarnのインストール  
下記のコマンドでインストールしてください  
`npm i -g yarn`

4. パッケージのインストール  
下記のコマンドでインストールしてください  
`yarn install`

お疲れ様でした、これで開発の準備は整いました  

## packageの説明
- 開発は`src`フォルダ内を編集してください
- 開発を始める前に必ず`yarn start`を叩いてからスタートしてください
これを叩くとwatchがスタートして変更をすぐにブラウザに反映してくれます
- watchされたファイルは`dist`フォルダに出力されます
- `src`フォルダ内のファイルを削除しても`dist`フォルダ内のファイルは削除されないので削除したい場合は`cmd + c`一旦処理を止め、再度`yarn start`を叩けば削除されます
- 使用するエディタで`.editorconfig`をオンにしてください
- 開発が完了し、公開する場合は`export`コマンドを叩いて`htdocs`のファイルを使用してください
`dist`フォルダ内との違いは`map`ファイルが削除され、`css`、`js`が圧縮されています
- htmlのlinetrは`htmlhint`を使用しています
- cssのlineterは`stylelint`を使用し、ルールは`stylelint-config-standard`を適用しています
- jsのlineterは`eslint`を使用し、ルールは`standard`を適用しています

## コマンド
`yarn run ◯◯`で実行してください  
※startは`yarn start`で実行できます  
|コマンド|説明|
|start|開発を始める前に実行  ファイルがwatchされ自動に反映される|
|export|htdocsフォルダに出力する|
|lint|lintチェックが実行されます|
|lintfix|エラー箇所をできるだけ自動で修正してくれます|
|format|htmlは.editorconfigルールにそって修正される + lintfix|
