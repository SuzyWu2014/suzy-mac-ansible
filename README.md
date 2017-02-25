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

Edit `roles/brew-pkgs-and-apps/defaults/main.yml`

```yaml
  homebrew_installed_packages:
    - wget
    - tree
    - ntfs-3g
    - mysql
    - python3
    - pyenv
    - node
    - zsh
    - zsh-completions
    - vim

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
```

Additional Configurations:
- Sublime Text 3
- oh my zsh

