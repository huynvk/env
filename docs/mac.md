# This is to define setup for mac os environment

## brew
Install follow guideline on its official site at [https://brew.sh/]

> /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

## iTerm2
Install iTerm2 via brew cask
> brew cask install iterm2

Setup natural text editing

> Preferences > Profiles > Keys  
> Load Presets... > Natural Text Editing

Download and install font Meslo at [https://github.com/powerline/fonts/blob/master/Meslo%20Slashed/Meslo%20LG%20M%20Regular%20for%20Powerline.ttf]

Change font for iTerm2 to the downloaded font
> iTerm2 > Preferences > Profiles > Text > Change Font

Set vertical cursor
> iTerm2 > Preferences > Profiles > Text  
> Cursor: Vertical Bar  
> Blinking Cursor: ON

## Zsh and Oh my Zsh

Install Zsh and zsh-completions
> brew install zsh zsh-completions

Install Oh my Zsh [github.com/robbyrussell/oh-my-zsh]
> sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Add Powerlevel9k Zsh Theme
> git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k  
> vi ~/.zshrc

Update the .zshrc file
> ZSH_THEME="powerlevel9k/powerlevel9k"

Add these lines into ~/.zshrc file
```
POWERLEVEL9K_PROMPT_ON_NEWLINE=true
POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(dir rbenv vcs)  
POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS=(status root_indicator background_jobs history time)  

# Add a space in the first prompt
POWERLEVEL9K_MULTILINE_FIRST_PROMPT_PREFIX="%f"
# Visual customisation of the second prompt line
local user_symbol="$"
if [[ $(print -P "%#") =~ "#" ]]; then
    user_symbol = "#"
fi
POWERLEVEL9K_MULTILINE_LAST_PROMPT_PREFIX="%{%B%F{black}%K{yellow}%} $user_symbol%{%b%f%k%F{yellow}%} %{%f%}"
```

Config Auto Suggestion
> git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions  

Add below flug in to .zshrc
```
plugins=(
    …
    zsh-autosuggestions
)
```

Config syntax highlight:
> brew install zsh-syntax-highlighting

Change vim color scheme: 
> vim ~/.vimrc  
> syntax on  
> colo koehler  

See more config for Zsh and Oh my Zsh at [https://medium.com/@Clovis_app/configuration-of-a-beautiful-efficient-terminal-and-prompt-on-osx-in-7-minutes-827c29391961]

## Node packages
### Node js
> brew install node

### Eslint