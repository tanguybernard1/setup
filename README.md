## setup MacOS workstation

### [Homebrew](https://brew.sh/index_fr)

```sh
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

```sh
  brew tap \
    heroku/brew \
    homebrew/cask \
    homebrew/cask-versions
```

```sh
  brew install \
    asdf \
    git \
    heroku \
    nginx \
    postgresql \
    sqlite \
    zsh \
    zsh-completions
```

```sh
  brew cask install \
    atom \
    docker \
    dashlane \
    firefox-developer-edition \
    firefox-nightly \
    google-chrome \
    google-chrome-canary \
    gpg-suite-no-mail \
    iterm2 \
    rubymine \
    spotify \
    tunnelblick
```

### [Oh-My-Zsh](https://ohmyz.sh/)

```sh
  sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### [zsh-completions](https://github.com/zsh-users/zsh-completions)

```
  rm -f ~/.zcompdump; compinit
  chmod go-w '/usr/locale/share'  
```

### .dotfiles

```sh
  bin/setup
```

### [SSH Key](https://help.github.com/en/enterprise/2.16/user/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

```sh
  ssh-keygen -t rsa -b 4096 -C 'beaurain.florent@gmail.com'
  eval "$(ssh-agent -s)"
  ssh-add -K ~/.ssh/id_rsa
```

### [GPG Key](https://help.github.com/en/articles/generating-a-new-gpg-key)

```sh
  gpg --full-generate-key
```