# Muxu Onboarding

Here you can find resources to setup your machine as a developer.

## Prerequisites

On OSX, first, you need to accept the developer license, to do that launch Xcode and follow the process.

Next, fire up your favorite terminal and install:

  - [Oh my zsh](https://github.com/robbyrussell/oh-my-zsh)
  - [brew](https://brew.sh/index_fr.html)
  - [npm](https://www.npmjs.com/)
  - [rbenv](https://github.com/rbenv/rbenv)
  - [ruby](https://www.ruby-lang.org/fr/) with `rbenv`
  	- `rbenv install 2.4.0`
  - [bundler](http://bundler.io)
  - [tmate](https://tmate.io/)
  - [jargon](https://github.com/muxumuxu/jargon)

Configure your SSH Keys with GitHub:

  - [Setup](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)
  - [Configure](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)

## Use [Middleman](https://middlemanapp.com/) for static websites

```
gem install middleman
middleman init MY_PROJECT -T git@github.com:muxumuxu/muxu-middleman-template.git
```

This middleman template is configured with [Sass](http://sass-lang.com/) and [Slim](http://slim-lang.com/).

## Use [Rails](http://rubyonrails.org/) for complex websites

First you need [Docker](https://docs.docker.com/docker-for-mac/install/) to be installed and running.

```
gem install rails # Install the latest rails version
rails new my_app -m https://raw.githubusercontent.com/muxumuxu/muxu-rails-template/master/template.rb
```

With those tools you should be able to develop anything ;)
