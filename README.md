----
**更新状況**
- 2018年5月22日(火) リポジトリ作成
- 2018年5月24日(木) 初版アップロード
- 2018年5月26日(土) Markdownガイド追加
- 2018年5月28日(月) MarkdownガイドにVSCodeでのやり方を追記
----

## GPIO早見表
<div align="center">
  <img src=./img/gpio.png>
</div>

## 各担当ドキュメント
- [Markdown使用の準備](./doc/markdown_guide.md)
- [通信機能](./doc/REST.md)
----

## GitHub操作のフローチャート

<div align="center">
  <img src=./img/git_guide.jpg>
</div>

<br>

上記画像はザックリとしていますが、[Gitの基本操作](https://github.com/gn5r/tutorial#Gitの基本操作)で初期化からローカルとリモートの関連付けをし、masterブランチのリポジトリをpullすることから始まります。<br>
Git操作コマンドリストを列挙してあるので、[こちら](https://github.com/gn5r/tutorial/blob/master/doc/git_command.md)(クリックでページ表示)も併せて目を通しておいてください。<br>
以下、箇条書きで手順を説明すると

1. 各自PCにGit用ディレクトリ作成
2. git関連づけるための初期化、リモートリポジトリ追加
3. GitHubで作成したリポジトリは全て**master**なので、`git pull リモート名 master` で更新
4. `git checkout -b ブランチ名`にて、各自ブランチを作成
5. 新規追加や変更をした場合、対象ファイル・ディレクトリをadd,commit
6. `git push リモート名 ブランチ名`で各自リモートへ適用(この時点ではmasterには適用されていない)
7. masterに適用してもらうため、Pull Request送信(Web上で行います)
8. masterがリクエストを許可した場合、変更内容が適用され結合される(masterリポジトリ内容が最新状態)
9. masterリポジトリの変更を適用するため、3と同じ手順を踏む(随時masterリポジトリは確認すること)
10. 変更・結合を繰り返し、masterリポジトリでは、各担当の完成したソースコートが列挙されている形になる(随時テストも行います)
11. 早く完成した場合はその都度、他の機能と結合しデバイスプログラムの完成形へ
12. 各機能を結合し、デバイスプログラムの完成

なお、当記事作者のブランチ名は **`gn5r`** です。<br>
また、ブランチ名はGitユーザー名と同じである必要は無く、短めの名前をおすすめします
