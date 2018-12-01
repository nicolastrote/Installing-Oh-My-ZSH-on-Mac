# MY ZSH CONFIGURATION AND TEMPLATE
Installation and template for my zsh

## PRELEMINARY: HOMEBREW INSTALLATION
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew -v
```
or if you have already brew installed
```
$ brew update
```

## INSTALLATION ZSH
```
$ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## INSTALLATION POWEERLINE9K THEME
And installation for a "powerline" style
```
$ git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
```
edit .zshrv config file and change the theme name : 
```
$ nano ~/.zshrc
  ZSH_THEME="powerlevel9k/powerlevel9k"
```

## INSTALLATION POWERLINE FONTS
I choose a programmer font. There is Adobe Source Code Pro and Source Code Pro, I will go with Adobe Source Code Pro. Both use some additional glyphs from Font Awesome, for that we need to edit .zshrv config file and insert just before the theme name, the POWERLEVEL9K_MODE property : 
```
$ nano ~/.zshrc
  POWERLEVEL9K_MODE='awesome-fontconfig'
  ZSH_THEME="powerlevel9k/powerlevel9k"
```
Next https://github.com/adobe-fonts/source-code-pro tell to execute:
```
$ brew tap caskroom/fonts && brew cask install font-source-code-pro
```
TERMINAL > preferences > profils > Police > modifed...
choose source-code-pro   13px
