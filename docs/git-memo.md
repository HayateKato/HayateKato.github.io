---
layout: page
title: "git memo"
permalink: /docs/git-memo
---

# gitの特徴
- 分散管理型のバージョン管理システム
- 元々はオープンソースソフトウェア管理のためのソフトウェアであった
- 変更履歴が残る
- 変更した箇所に戻ることができる
- 他人と共同編集できる

# gitが持つ機能
## コミット
### ファイルの作成，変更，削除の記録を行う
- いつ・誰が・何を・どのような
- コミットにメッセージを残す（「どのような」を記載）
### 対象ファイルは1つでも複数でもよい
### コミットの単位はユーザが自由に決定する

## レポジトリ
### gitが管理するプロジェクトのフォルダ
- ローカルレポジトリ･･･個々のプロジェクト実行環境
- リモートレポジトリ･･･共有の管理場所（Github/Gitlabなど）

## ブランチ
### 作業を枝分かれさせることができる
- 共同作業・並行作業が可能

# gitのコマンド
## git config --global user.name yourname@example.com
- ホスト（OS）全体のgitの設定
## git symbolic-ref HEAD refs/heads/main
- HEAD（ローカルレポジトリでの最新の状態）をmainと設定する
## git branch --set-upstream-to origin/main
- リモートブランチ（origin/main）と紐付ける設定
- -originはリモートでのデフォルトのサーバー
## git stash
- 一時退避
## git diff origin -- index.html
- -originにあるindex.htmlとローカルのindex.htmlの比較
## git pull
- -originからプル（同期）
## git stash pop
- 一時退避したものに変更を加える
##git merge --abort
- mainブランチをマージを試行する前の状態に復元
## git reset --hard
- マージを開始する前の状態に戻す
## git init
- gitの初期化・設定開始
## git status
- ワークツリーのステータスを表示
## git config
- 設定周りの確認・変更
## git log
- ログを表示（-- onlineでコミットメッセージの1行のみの一覧表示）
## git diff
- ファイルの差分を表示
## git add
- ステージングエリアに追加
## git commit
- コミットの実行
## git commit --amend --no-edit
- コミットの修正
## git reset
- コミットのリセット
## git revert
- 「コミットの変更を打ち消す」コミット
## git rm
- ファイルとindex情報の削除
## git clone
- レポジトリをコピー
## git pull
- リモートレポジトリの同期
## git push
- 変更をアップロードする
## git request-pull
- プルリクエスト（変更依頼）
## git remote
- リモートレポジトリの設定
## git branch
- ブランチの作成
## git checkout
- ブランチの切り替え
## git merge
- ブランチの統合