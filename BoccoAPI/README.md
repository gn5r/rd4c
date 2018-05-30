# 本型デバイス通信機能

**更新履歴**
- 2018年5月24日(木) 初版アップロード
- 2018年5月30日(水) ディレクトリ移動、ライブラリ化するプログラムを公開
- 2018年5月31日(木) bocco4jのライブラリ化。maven及びGradleから参照可能
----

## プログラム本体
[bocco4j](https://github.com/gn5r/bocco4j)にライブラリ化するプログラムをPushしました。どういう動作をしているのか見たかったら覗いて見てください。<br>
なお、このライブラリをインポートするにはpom.xmlに以下を追記

```pom.xml
<repositories>
  <repository>
      <id>jitpack.io</id>
      <url>https://jitpack.io</url>
  </repository>
</repositories>

<dependency>
  <groupId>com.github.gn5r</groupId>
  <artifactId>bocco4j</artifactId>
  <version>-SNAPSHOT</version>
</dependency>
```

## 実装予定機能
- セッション情報を作成し、AccsessTokenを取得
- 取得したAccsessTokenを使い、Bocco本体へPost
- 必要であるならアプリも作成し、ルームにどのように送信されるかを確認
- チャットルーム情報取得
- チャットルームへのメッセージ送信機能
- チャットルームのメッセージ取得機能

## デバイスプログラムでのフローチャート

<div align="center">
  <img src=../img/rest_flow.jpg>
</div>

## 必要なもの
- Bocco本体
- Bocco REST APIの登録
