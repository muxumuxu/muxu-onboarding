# Muxu Onboarding

Here you can find resources to setup your machine as a developer.

## Prerequisites

On OSX, first, you need to accept the developer licence, to do that launch Xcode and follow the process.

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
  - [Hub](https://github.com/github/hub)

Next alias `git` to use `hub`:
```
echo 'eval "$(hub alias -s)"' >> ~/.zshrc
```
And restart your shell.

Configure your SSH Keys with GitHub using this [link](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/).

## Use [Middleman](https://middlemanapp.com/) for static websites

```
gem install middleman
middleman init my_app -T git@github.com:muxumuxu/muxu-middleman-template.git
git init
git add .
git commit -m "Initial Muxu.Muxu middleman app"
git create -p muxumuxu/my_app
```

This middleman template is configured with [Sass](http://sass-lang.com/) and [Slim](http://slim-lang.com/).

#### Custom Domain + SSL with GitHub pages

- Create your domain on [Cactomain](https://cactomain.co/register)
- Configure *Named Servers* with 
  - `ken.ns.cloudflare.com`
  - `tegan.ns.cloudflare.com`
- Add a new website on [Cloudfare](https://www.cloudflare.com/a/add-site) and wait to be correctly recognized
- Once done, go to DNS section of Cloudfare and add two DNS records
  - `A @ 192.30.252.153`
  - `A @ 192.30.252.154`
- Add custom domain to your GitHub repository
- You should be OK

## Use [Rails](http://rubyonrails.org/) for complex websites

First you need [Docker](https://docs.docker.com/docker-for-mac/install/) to be installed and running.

```
gem install rails # Install the latest rails version
rails new my_app -m https://raw.githubusercontent.com/muxumuxu/muxu-rails-template/master/template.rb
git create -p muxumuxu/my_app
```
