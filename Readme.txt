[参考]
　https://backlog.com/ja/git-tutorial/reference/

origin/master
　リモートリポジトリ「origin」のブランチ「master」の位置を表しています。
origin/HEAD
　リモートリポジトリ「origin」をクローンした時にダウンロードされるコミットの位置を表しています。
　通常「origin/master」と同じ位置を指します。
master
　ローカルリポジトリのブランチ「master」の位置を表しています。
origin
　クローンした場合、どこのツリーを取得したかの情報が"origin"として記録されます。
stash
　ファイルの変更内容を一時的に記録しておく領域です。

fast-forward(早送り)マージ
　masterブランチは単純に移動するだけのマージ。
non fast-forwardマージ
　fast-forwardマージが可能な場合でも新しくマージコミットを作成して合流させること。
merge
　変更内容の履歴はそのまま残るが、履歴が複雑になる。
rebase
　履歴は単純になるが、元のコミットから変更内容が変更される。
　そのため、元のコミットを動かない状態にしてしまうことがある。
　mergeとrebaseは、チームの運用方針に応じて使い分けます。
　例えば、履歴を一本化するように運用をするのであれば
　・トピックブランチに統合ブランチの最新のコードを取り込む場合はrebaseを使う
　・統合ブランチにトピックブランチを取り込む場合は、まずrebaseしてからmerge

A successful Git branching model
　http://keijinsonyaban.blogspot.com/2010/10/a-successful-git-branching-model.html

fetch
　リモートリポジトリの最新の履歴の取得だけを行うことができます。
pull
　fetch + merge

amendオプション
　同じブランチの直前のコミットに対して内容を追加やコメントの修正をすることができます。
revert
　指定したコミットの内容を打ち消すコミットを作り出すことができます。
reset
　要らなくなったコミットを捨てることができます。
cherry-pick
　別のブランチから指定したコミットをコピーして、現在のブランチに取り込む事ができます。
