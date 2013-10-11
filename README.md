ccsd_2013
=========

事前準備
-----
+ [Vagrant環境のセットアップ](https://github.com/ychubachi/vagrant_enpit_package "ychubachi/vagrant_enpit_package")


このブランチで行うテストの内容
-----

###Vagrantの開始・SSH接続###
  ```
  $ vagrant up
  $ vagrant ssh
  $ cd /vagrant/work
  ```
  
###レポジトリのクローン###
  ```
  $ git clone git@github.com:ychubachi/ccsd_2013.git
  $ cd ccsd_2013
  ```

###他の人の行なった編集の取り込み###
  ```
  $ git fetch
  $ git merge origin/master
  ```

###コンソールでの編集###
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

###GitHubでの操作###

1. https://github.com/ychubachi/ccsd_2013 のbranchesから自分のブランチ名をクリック  
2. 右上の「merge & pull request」という緑色のボタンを押下  
3. mergeされるのを待つ
