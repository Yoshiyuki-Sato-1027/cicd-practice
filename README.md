## actionlint について

TODO
`actionlint`を pre-commit 時にする

## GithubActions の CICD ワークフローの書き方を学習する

## コンテキスト

# github コンテキスト

- run: echo "${{ github.actor }}" # github コンテキストの参照

# runner コンテキスト

# 環境変数

github コンテキストと内容一緒

- run: echo "${GITHUB_ACTOR}" # コンテキストではなくデフォルト環境変数を指定

# Variables

環境変数 UserName に Variables で登録した値を格納している
env:
USERNAME: ${{ vars.USERNAME }} # Variables の参照

# Secrets

# ステータスチェック関数

success()：手前の処理が成功したら true
failure()：手前の処理が失敗したら true
cancelled()：手前の処理がキャンセルされたら true
always()：手前の処理結果を問わず常に true
