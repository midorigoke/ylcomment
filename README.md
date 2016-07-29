# ylcomment
Youtube Liveのコメントを取得するシェルスクリプト

## 使い方
1. jqをインストールする
1. $ git cloneとかでダウンロードする
1. まず実行する
1. [Google API Manager](https://console.developers.google.com)でAPIキーを取得する
1. ~/.ylconfigを編集してAPIキーを書き込む
1. 引数に動画ID(YoutubeのURLのV=の部分)を与えて実行する

## 注意
* これはコメントを取得するだけです。
読みあげたい場合は別途読み上げソフトを用意してパイプ等で渡してあげてください。
* 最初に放送開始時のコメントまでさかのぼって取得してその後は差分を出力します。
なので放送途中に取得を開始するとそれ以前のコメントが大量に流れます。