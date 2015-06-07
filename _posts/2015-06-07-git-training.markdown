---
layout: post
title:  "git training (2)"
date:   2015-06-05 12:30:00
categories: git
---

GitHub "GIT CHEAT SHEET"を参照

# グループを変更する

{% highlight ruby %}
# ローカルのブランチを一覧する
git branch

# ブランチを作成する
git branch [branch-name]

# 現在のブランチを指定したブランチに変更する
git checkout [branch-name]

# 指定したブランチの変更を現在のブランチに適用する
git merge [branch-name]

# 指定したブランチを削除する
git branch -d [branch-name]

{% endhighlight %}

# 変更を戻す

{% highlight ruby %}
# ファイルを現在のディレクトリ及びプッシュ先のリポジトリから削除する
git rm [file-name]

# ファイルをプッシュ先のリポジトリからは削除し、現在のディレクトリからは削除しない
git rm --cached [file-name]

# ファイルネームを変更し、コミットと比較する
git mv [file-name-original] [file-name-renamed]

{% endhighlight %}

# 断片的に保存する

{% highlight ruby %}

# 一時的にすべての修正を加えたファイルを退避させる
git stash

# 一時的に保存したファイルを戻す
git stash pop

# stashしているファイルを一覧する
git stash list

# 最後にstashしたファイルを削除する
git stash drop

{% endhighlight %}

# 履歴を確認する

{% highlight ruby %}

# 現在のブランチに関する過去のコミットを一覧する
git log

# 特定のファイルについて、現在のブランチに関する過去のコミットを一覧する
git log --follow [file-name]

# 選択した二つのブランチの差異を確認する
git diff [first-branch-name] [second-branch-name]

# 特定のコミットに関する情報を閲覧する
git show [commit-id]

{% endhighlight %}

# 変更を同期する

{% highlight ruby %}

# 指定したブックマークのすべての履歴をダウンロードする
git fetch [bookmark-name]

# 指定したブックマーク・ブランチの変更を現在のブランチに適用する
git merge [bookmark-name]/[branch-name]

# すべてのコミットをプッシュする
git push

# 現在のブックマークの変更履歴をダウンロードし、現在のブランチに適用する
git pull

{% endhighlight %}
