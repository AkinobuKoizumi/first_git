git push の実験です。

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


以下を参考に設定しました。
https://prog-8.com/docs/git-env