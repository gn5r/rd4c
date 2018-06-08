# 本型デバイス通信機能

**更新履歴**
- 2018年5月24日(木) 初版アップロード
- 2018年5月30日(水) ディレクトリ移動、ライブラリ化するプログラムを公開
- 2018年5月31日(木) bocco4jのライブラリ化。maven及びGradleから参照可能
- 2018年6月3日(日)  開発時の参考サイトを記載
- 2018年6月4日(月)  ライブラリ完成
----

## 参考サイト
- [HttpURLConnection で POST リクエスト](http://a4dosanddos.hatenablog.com/entry/2015/12/18/012353)
- [JavaからJSON文字列をPOSTで送信する](http://suzu6.hatenablog.com/entry/2017/09/21/234704)
- [URLConnection(HttpURLConnection)と向き合おう~POSTメソッドでJSONを送信する~](http://blog.officekoma.co.jp/2016/08/urlconnectionhttpurlconnectionpostjson.html)

## プログラム本体
[bocco4j](https://github.com/gn5r/bocco4j)にライブラリ化するプログラムをPushしました。どういう動作をしているのか見たかったら覗いて見てください。<br>
なお、このライブラリをインポートするにはpom.xmlに以下を追記

``` xml
<repositories>
  <repository>
      <id>jitpack.io</id>
      <url>https://jitpack.io</url>
  </repository>
</repositories>

<dependencies>
  <dependency>
    <groupId>com.github.gn5r</groupId>
    <artifactId>bocco4j</artifactId>
    <version>-SNAPSHOT</version>
  </dependency>
</dependencies>
```

## 実装機能
- セッション情報を作成し、AccsessTokenを取得
- 取得したAccsessTokenを使い、roomIDを1件取得
- 取得したAccessTokenとroomIDを使い、ルームへメッセージを送信

## デバイスプログラムでのフローチャート

<div align="center">
  <img src=../img/rest_flow.jpg>
</div>

## 必要なもの
- Bocco本体
- Bocco REST APIの登録
