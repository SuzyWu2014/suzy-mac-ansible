# suzy-mac-ansible
Ansible roles to set up my Mac OS X

## Prerequisite

+ Install Apple's commandline tool: `xcode-select --install`
+ Ansible

```
sudo easy_install pip
sudo pip install ansible
```

## Included Applications / Configuration

Modify `roles/brew-pkgs-and-apps/defaults/main.yml` as needed.

```yaml
  homebrew_installed_packages:
    - wget
    - tree
    - mysql
    - python3
    - pyenv
    - node
    - zsh
    - zsh-completions
    - vim
    - homebrew/fuse/ntfs-3g

  homebrew_upgrade_all_packages: no

  homebrew_taps:
    - homebrew/core
    - caskroom/cask

  homebrew_cask_apps:
    - firefox
    - google-chrome
    - iterm2
    - slack
    # sublime text 3 by default
    - sublime-text
    - grammarly
    - the-unarchiver
    # java 8
    - java
    - docker
    - virtualbox
    - vagrant
    - vagrant-manager
    - evernote
    - texmaker
    - qlmarkdown
    - quicklook-json
    - osxfuse
    - pycharm

  homebrew_cask_appdir: /Applications
```

## Manual Configurations

### Applications

+ Install `BetterSnapTools`

### Iterm2 Appearance

+ 1. Change bash to zsh. `chsh zsh `

### Sublime Text 3

See [Sublime Text 3 Configuration](http://suzywu2014.github.io/ubuntu/2017/02/18/Ubuntu-sublime3)
