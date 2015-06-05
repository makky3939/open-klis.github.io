---
layout: post
title:  "git training"
date:   2015-06-05 12:30:00
categories: git
---

GitHub "GIT CHEAT SHEET"を参照

# 設定をする　

{% hilight shell%}

# 名前を設定
git config --global user.name "your name"

# メールアドレスを設定
git config --global user.email "your email address"

{% endhighlight %}

# リポジトリを作る

{% hilight shell%}

# リポジトリを作成
git init

# リポジトリをクローン
git clone [repository's url]

{% endhighlight %}

# 変更を加える

{% hilight shell%}

# コミットされたファイルのリストを見る
git status

# Shows file differences not yet staged (訳求む)
git diff

# コミットするファイルを追加する
git add [file]

# プッシュ前のファイルを取り消す(訳求む)
git reset [file]

# コミットする
git commit -m 'commit message'

