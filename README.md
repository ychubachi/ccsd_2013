ccsd_2013
=========

このブランチで行うテストの内容
-----

###レポジトリのクローン###
  ```
  $ vagrant up
  $ vagrant ssh
  $ cd /vagrant/work
  $ git clone git@github.com:ychubachi/ccsd_2013.git
  $ cd ccsd_2013
  ```

###コンソールでの編集###

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
