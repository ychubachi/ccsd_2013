ccsd_2013
=========

事前準備
-----
+ [Vagrant環境のセットアップ](https://github.com/ychubachi/vagrant_enpit_package "ychubachi/vagrant_enpit_package")


このブランチで行うテストの内容
-----

###Vagrantの開始・SSH接続
  ```
  $ vagrant up
  $ vagrant ssh
  $ cd /vagrant/work
  ```
  
###レポジトリのクローン
  ```
  $ git clone git@github.com:ychubachi/ccsd_2013.git
  $ cd ccsd_2013
  ```

###他の人の行なった編集の取り込み
  ```
  $ git fetch
  $ git merge origin/master
  ```

###コンソールでの編集
自分のブランチの作成
  ```
  $ git checkout -b <自分のID>
  ```
エディタを使って<自分のID>.htmlを作成
  ```
  $ vim <自分のID>.html
  ```
変更内容をstage
  ```
  $ git stage <自分のID>.html
  ```
変更内容をcommit
  ```
  $ git commit -m "<コメント>"
  ```
自分のブランチをリモートに作成
  ```
  $ git push -u origin <自分のID>
  ```

###GitHubでの操作
1. https://github.com/ychubachi/ccsd_2013 のbranchesから自分のブランチ名をクリック  
2. 右上の「merge & pull request」という緑色のボタンを押下  
3. mergeされるのを待つ


覚えておいた方がいいGitコマンド
-----

###status
困ったらとりあえず叩くと今どうなってるのかが分かる。
  ```
  $ git status
  ```

###branch
ローカルのブランチを知るのに使える。
  ```
  $ git branch
  ```
また、`-a`オプションを付けることでリモートからfetchしてきたブランチ(`git merge`する時に指定するブランチ)の一覧も見ることができる。
  ```
  $ git branch -a
  ```

###log
現在のブランチのコミット履歴を見ることができる。
  ```
  $ git log
  ```

###remote
`git push`や`git fetch`を行うときのリモートブランチを操作できる。  
`-v`オプションを付けることで、addしているリモートブランチの一覧を見ることができる。
  ```
  $ git remote -v
  ```
`remote add`コマンドによって新しいリモートレポジトリを追加できる。
  ```
  $ git remote add <リモートレポジトリのタグ名> <リモートレポジトリのURL>
  ```
