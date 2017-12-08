---
layout: post
title:  "Welcome to Jekyll!!"
date:   2017-12-07 12:33:19 +0000
categories: jekyll
---
It's my very first entry on that blog. I tried to run a few previously but without any success ;)
Let'see if this time it'll look differently.

I choose Jekyll to learn something new and use GitHub to host my blog. I'm using Ubuntu for my everyday work so I would like to have that first post usable some information about starting using Jekyll on Ubuntu machine.

**Don't do sudo apt-get install gem** :)

Instead:

* Install Ruby [https://coderwall.com/p/0o64yq/rbenv-issues-when-switching-to-zsh]:
{% highlight bash %}
cd $HOME
sudo apt-get update 
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL
git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL
​
rbenv install 2.4.2
rbenv install 2.4.2
ruby -v
{% endhighlight %}
* If you switched to ZSH in mean time [​https://coderwall.com/p/0o64yq/rbenv-issues-when-switching-to-zsh]:
{% highlight bash %}
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshenv
echo 'eval "$(rbenv init -)"' >> ~/.zshenv
echo 'source $HOME/.zshenv' >> ~/.zshrc
exec $SHELL
{% endhighlight %}
* Install Jekyll
`gem install jekyll bundler`
* Start it:
`bundle exec jekyll serve`

And you should see something in browser when you open http://localhost:4000.

[https://coderwall.com/p/0o64yq/rbenv-issues-when-switching-to-zsh]: https://coderwall.com/p/0o64yq/rbenv-issues-when-switching-to-zsh
[​https://coderwall.com/p/0o64yq/rbenv-issues-when-switching-to-zsh]: https://coderwall.com/p/0o64yq/rbenv-issues-when-switching-to-zsh