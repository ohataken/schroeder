## コード中のコメントについて

- コード中にコメントは書かない

## git commit について

- Claude が working directory を書き換えたら commit する
    - ユーザーはコードを Git クライアントを使って読んでいる
- commit の粒度について
    - ユーザーのレビューのしやすさのため、粒度は小さい方がよい
    - メソッドやブロックごとの粒度がよい
    - 複数のファイルやディレクトリにまたがる変更の場合は、その意味のまとまりごとの粒度にする
    - commit ごとに build, lint が通らなくてもよい。pull request 単位でそれらが通ればよい
    - package manager, task runner, build tool などが自動生成する変更と、それ以外の一般的なコードの変更は別の commit として分ける
- commit message について
    - Conventional Commits の形式に従う
    - その上でリポジトリごとの慣例に従う
