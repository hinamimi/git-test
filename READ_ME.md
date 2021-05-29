# Gitを学ぼう

1. Gitの概念を知ろう
    - 分散型バージョン管理システム
    - ブランチによる機能ごとの管理
2. Git特有のキーワード
   - リポジトリ
   - ステージ
   - HEAD
   - origin
3. Gitによる管理の流れ
    1. `git clone`でリポジトリをローカルに保存 (または`git init`でローカルレポジトリを作成)
    2. `git branch`で新規ブランチを作成、`git checkout`で移動して、機能追加・機能修正のためのファイルを編集
    3. `git add`・`git commit`を繰り返し実行し、機能を追加
    4. `git pull`でリモートレポジトリの変更を確認、（場合によっては）コンフリクト解消(`git pull`=`git fetch`+`git merge`)
    5. `git push`してリモートレポジトリに変更を反映
    6. `pull request`を発行、レビューを依頼
    7. 公式にマージ(またはフィードバックを元に3に戻る)
4. Github flowについて
    - `main`ブランチと`feature/XXX`ブランチを使用する
    - もし間違えたブランチにコミットしてしまったら
        - `git reset --soft HEAD^` -> `git stash` -> `git checkout ${branch}` -> `git stash pop`
5. `commit`のまとまりについて
    できるだけまとまったひとつの作業に対してコミットする
        Aの変更しながら、その付近のBのコードをリファクタリングした  
            -> まとめてコミット △  
            -> `git add -p`などを使ってAのコミットとBのコミットで分ける
        
6. ハンズオンでやってみよう
    1. `git clone https://github.com/hinamimi/git-test.git`
    2. `git branch feature/$``git checkout feature/${function-name}`
    3. `hand_on.md` -> `hand_on.html`
        - exampleは答えの例、わからんかったとき用