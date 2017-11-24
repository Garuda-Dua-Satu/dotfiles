# dotfiles
My collection of dot files

## Tools
- ubuntu
- terminator
- zsh
- vim
- tmux
- rvm + ruby

## Oh My ZSH
```bash
cd
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Powerline Font
```bash
cd
git clone https://github.com/powerline/fonts.git --depth=1
./fonts/install.sh
rm -rf fonts
```

after that change font in terminal to any of powerline font

## Solarize Theme
```dconf``` is required for ubuntu
```bash
sudo apt-get install dconf-cli
```

```bash
git clone git://github.com/sigurdga/gnome-terminal-colors-solarized.git ~/.solarized
cd ~/.solarized
./install.sh
```
- Choose **option 1** (dark theme).  
- Choose **option 1** to download seebi' dircolors-solarized

To activate dark solarize theme in Terminator just right click on the terminal, 
> Preferences>Profiles>Colors>Foreground and Background>Built-in schemes: Solarized dark
> Preferences>Profiles>Colors>Palette>Built-in schemes: Solarized

Restart Terminator and you're done!

## Additional
##### RVM users
```bash
RPROMPT="\$(~/.rvm/bin/rvm-prompt s i v g)%{$fg[yellow]%}[%*]"
```
##### Rbenv users
```bash
RPROMPT='%{$fg[yellow]%}$(rbenv version-name)%{$reset_color%}%'
```

##### Vundle
```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

##### Silver Searcher
Ag is faster than ack

```bash
sudo apt-get install silversearcher-ag # ubuntu
brew install the_silver_searcher # macos
```

##### Youcompleteme
```bash
sudo apt-get install build-essential cmake3 # cmake on >= 16.04
cd ~/.vim/bundle/YouCompleteMe
./install.py --cs-completer --js-completer --go-completer
```

##### Fuzzy Finder
```bash
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install
```
