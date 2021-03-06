# Gitについて

## gitの初期化
$ git init

## git管理から除外するファイルの設定
.gitignoreに記載

## ローカルブランチを表示
$ git branch

## リモートブランチを表示
$ git branch -r

## ローカル・リモート全てのブランチを表示
$ git branch -a

## ブランチの移動
$ git checkout <移動先ブランチ名>

## リモートのhogeブランチをローカルに作成
$ git checkout -b <ローカルブランチ名> origin/hoge

## 変更ファイルの一覧を表示
$ git status

## ステージングエリアに追加
$ git add <File Name>
「*.txt」のようにワイルドカード使用可能
「.」にするとサブディレクトリを含む全てのファイルをステージングエリアに追加

## コミット
$ git commit -m "<Commit Message>"

## コミットログを表示
$ git log

## コミットログを1行で表示
$ git log --oneline

## コミットログをグラフで表示
$ git log --graph

## remoteのサーバ名(URL)を「origin」に設定
$ git remote add origin <Remote RepositoryのURL>

## remoteのサーバ名表示
$ git remote -v

## remoteのmasterにlocalのmasterをPushする
$ git push origin master

## コミットをまとめる
// 直近3件の場合<br>
$ git rebase -i HEAD~3<br>
// エディタが表示されるのでログを操作する。

