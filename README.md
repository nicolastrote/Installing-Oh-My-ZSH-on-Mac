# MY ZSH CONFIGURATION AND TEMPLATE
![alt text](https://github.com/nicolastrote/MY-ZSH-CONFIG/blob/master/ntrote-zsh-color.png)

Installation and template for my zsh:
 * zsh
 * oh-my-zsh
 * iTerm2
 * POWEERLINE9K theme Solarized: Light and Solarized Dark
 * POWERLINE fonts

## PRELEMINARY: HOMEBREW INSTALLATION
Brew is a package manager for OSX
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew -v
```
or if you have already brew installed
```$ brew update```

## INSTALLATION ZSH
```brew install zsh```

## INSTALLATION OH-MY-ZSH
```$ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"```

## INSTALLATION iTERM2
iTerm2 permet de faire du tilling!
Install iTerm2: https://iterm2.com/downloads/stable/iTerm2-3_1_6.zip

Indiquer à iTerm2 d'utiliser ZSH
 * go to iTerm2 preferences.
 * head to Profiles -> General.
 * paste /bin/zsh in the Command textbox and restart iTerm2.

For color download : 
 * https://raw.githubusercontent.com/mbadolato/iTerm2-Color-Schemes/master/schemes/Solarized%20Dark%20-%20Patched.itermcolors
 * https://raw.githubusercontent.com/altercation/solarized/master/iterm2-colors-solarized/Solarized%20Light.itermcolors
Term → preferences → profiles → colors → load presets

If you like my theme, you can download my color theme from the repository: [ntrote.itermcolors](https://github.com/nicolastrote/MY-ZSH-CONFIG/blob/master/ntrote.itermcolors)

## INSTALLATION POWEERLINE9K THEME
And installation for a "powerline" style
```$ git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k```
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
`$ brew tap caskroom/fonts && brew cask install font-source-code-pro`
 * Term → preferences → profiles > Police > modifed...
 * choose source-code-pro   13px
