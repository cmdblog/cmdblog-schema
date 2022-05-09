# ARCHIVED

このrepositoryは cmdblog/cmdblog-backendに統合されました。


# cmdblog-schema

backend サーバーの提供するAPI用のJSON schema

# リリースサイクル

ここを更新するたびに、release versionを切る。
他のrepositoryはversionを指定してこのschemaをimportして利用する。

# Contribution

0. `gh repo fork cmdblog/cmdblog-schema`でこのrepositoryをforkする (初回のみ)
0. `git checkout main` or `git switch main`でmainブランチに移動する
0. `git fetch upstream`でlocalのupstreamを更新する
0. `git rebase upstream/main`で、最新のupstream/mainをlocalのmainブランチに取り込む
0. `git checkout -b <わかりやすいブランチ名>` or `git switch -c <わかりやすいブランチ名>` で機能用ブランチを切る
0. コードに修正を加え、必要ならばテストを付ける
0. `make check-all` で問題がないことを確認し、`git commit git push` する
0. `gh pr create -w` で本repositoryへのPRを作成し、reviewersを指定する。
0. approveされた後、PR作成者がmergeボタンを押す。
    - 例外
        - PR作成者にmerge権限がない場合はPR作成者以外がmergeしてもよい。
        - PR作成者にmergeをしてもらうことが困難で、かつそのPRのmergeが他のタスクのボトルネックになっている際は、PR作成者以外がmergeしてもよい
0. PR画面からremoteの機能用ブランチを消す
0. `git cehckout main` or `git switch main` でmainブランチに戻り、`git fetch --prune git fetch -D <当該ブランチ名>` で、機能用ブランチを削除する
