6/17日報
# 学習内容
 GitHub ssh接続まで  
リファレンス作成  
サイト模写  
理解・発見・気付き  

- ssh -T git@github.com接続　によるエラー(Permission denied (publickey)  
結論：SSHキー名をgithub用に命名指定たためconfigに設定する必要がある  
クライアント側（Mac）へのSSHキーの設定(config内容)  
```
  $ vim ~/.ssh/config
    ~/.ssh/config
    Host github
    HostName github.com
    IdentityFile ~/.ssh/id_rsa ← 命名したものに変更する必要がある
    User git
```
わからなかったこと  
 参画した時にgithub初期設定操作はどこまでするのか伺いたいです  
公開鍵作成,githubに登録  
sshで接続  
clone取り込み  
ssh取り込んだ内容をコミット&プッシュ  

6/21
## その日何をやったか  
  - サイト模写  
    - html 基礎文法　テンプレ作成  
    - 引き継ぎ用のherokuドキュメント作成  
    - Finderにあるフォルダ整理  

## 理解したこと・発見・気づき
  - マークアップ  
    - id 記述一回　classは複数呼び出し  

## わからなかったこと

- BEM OOCSS SMACSS 記法でどれを意識して書いた方がよろしいでしょうか？？  
  - 現場によってであれば、現在booksmart_viewで記述しているものを参考にした方が良いですか？？