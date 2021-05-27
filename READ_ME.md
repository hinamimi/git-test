# Gitを学ぼう

1. Gitの概念を知ろう
    - 分散型バージョン管理システム
    - ブランチによる機能ごとの管理
2. Gitによる管理の流れ
    1. `git clone`でリポジトリをローカルに保存 (または`git init`でローカルレポジトリを作成)
    2. `git branch`で新規ブランチを作成、`git checkout`で移動して、機能追加・機能修正のためのファイルを編集
    3. `git add`・`git commit`を繰り返し実行し、機能を追加
    4. `git pull`でリモートレポジトリの変更を確認、（場合によっては）コンフリクト解消(`git pull`=`git fetch`+`git merge`)
    5. `git push`してリモートレポジトリに変更を反映
    6. `pull request`を発行、レビューを依頼
    7. 公式にマージ(またはフィードバックを元に3に戻る)
3. ハンズオンでやってみよう