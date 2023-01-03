ローカルからリモートにpushをする実験です。



初めての時
==============
1. gitで管理するディレクトリの作成
mkdir first_git
2. ディレクトリへ移動
cd first_git
3. 移動したフォルダをgitで管理するためのコマンドを実行する
git init
4. 現在のブランチをmainに変更する
git branch -M main
5. プッシュ先のリモートリポジトリの指定
git remote add origin git@github.com:AkinobuKoizumi/first_git.git
6. リモートリポジトリが登録できたか確認
git remote -v
7. コミットする
git add .
git commit -m "First Commit."
8. プッシュする
git push origin main




2回目以降の時
==============
1. アップロードしたいフォルダに移動
cd first_git
2. ステージング
git add -A
3. コミット
git commit -m 'add comment'
4. フェッチ（リモートリポジトリの最新の履歴を取得）
git fetch origin
5. マージ
git merge main
6. プッシュ
git push


ブランチへのpush方法
==============
git clone {{URL or SSH}}
git branch -a 
git checkout users/koizumi
git branch -a
git push origin users/koizumi


参考資料
==============
・初めての時
https://prog-8.com/docs/git-env
・2回目以降の時
https://zenn.dev/toshihide2000/articles/d0c99f96e2706a
・ブランチへのpush
https://qiita.com/infratoweb/items/5021a36f69f26dc7f0b9