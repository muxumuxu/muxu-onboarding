# Muxu Onboarding

Here you can find resources to setup your machine as a developer.

On OSX, first, you need to accept the developer license, to do that launch Xcode and follow the process.

Fire up your favorite terminal and install:

- [Oh my zsh](https://github.com/robbyrussell/oh-my-zsh)
- [brew](https://brew.sh/index_fr.html)
- [npm](https://www.npmjs.com/)
- [rbenv](https://github.com/rbenv/rbenv)
- [ruby](https://www.ruby-lang.org/fr/) with `rbenv`
	- `rbenv install 2.4.0`
- [bundler](http://bundler.io)
- [tmate](https://tmate.io/)

Configure your SSH Keys with GitHub:

- [Setup](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)
- [Configure](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)

Configure for static website with [middleman](https://github.com/muxumuxu/knowledge_base/blob/master/middleman.md):

```
gem install middleman
middleman init MY_PROJECT -T git@github.com:muxumuxu/muxu-middleman-template.git
```

With those tools you should be able to develop anything ;)
