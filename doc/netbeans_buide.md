# デバイスプログラム開発ガイド

## 開発機能の確認

現段階で開発する機能は以下の通りかと思います

- Boccoとのやり取りをする為の準備～メッセージなどのやり取り
- NFCリーダーを用いて、NFCタグ内の情報を読み取る
- マイクを使い録音し、ライブラリを使い音声から文字列化。スピーカーからBGMと効果音再生
- 各ボタン押下によるイベント処理

# 開発環境構築
本プログラムは **Java** で書いてもらおうかと思います。<br>
Java開発と聞くと、Eclipseを使う事が大体ですが、今回は比較的軽量な **NetBeans** を使い、開発してもらいます。<br>

## JDK8とNetBeansの導入
[JDK8公式サイト](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)より、**8u171** をダウンロードし、インストールしておいてください。<br>
[NetBeansダウンロードページ](https://netbeans.org/downloads/?pagelang=ja)にアクセスし、 **Java SE** をダウンロードしておいてください。<br>
PHP,HTML,JavaScript,C/C++に対応したIDEもありますが、今回の開発には必要ありません。<br>

JDK、NetBeansをインストールする際、ディレクトリを変更しても構いませんが、**十分に理解している** 場合のみでお願いします。<br>
基本的にはWindowsを使ってる限り、インストールディレクトリを変更する必要はありません。<br>

## NetBeansの初期設定
JDK8とNetBeansの導入が終わりましたら、コード補完の設定をします。<br>
[NetBeansでも爆速コーディング](http://masatoshitada.hatenadiary.jp/entry/2014/06/11/172203)を参考に、オプション→エディタ→コード補完からJavaを選択し、トリガーに`.abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_`を入力しておいてください。
