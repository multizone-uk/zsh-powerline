# Powerline for Zsh with architecture for people with a mixture of arm and x86 Macs and Linux computers.

Adds ` COLOR_ARCH` so that the prompt reminds you if you are running arm or x86.

```
# Colorscheme
readonly COLOR_CWD='magenta'
readonly COLOR_GIT='cyan'
readonly COLOR_SUCCESS='green'
readonly COLOR_FAILURE='red'
readonly COLOR_TIME='cyan'
readonly COLOR_ARCH='white'
```

Adds `arch` to `config_prompt`.
```
local arch="%F{$COLOR_ARCH}$(arch)%f"
```

Makes the prompt how I like it.
```
PROMPT="%n@%m $arch $cwd$git $symbol %# "
```
Comments out the right prompt.

# Forked from 

## zsh-powerline

Powerline for Zsh in pure Zsh script.
(https://github.com/riobard/zsh-powerline/).

### Installation

Download the Zsh script, from the multizone branch

```sh
curl https://raw.githubusercontent.com/multizone-uk/zsh-powerline/multizone/zsh-powerline.sh > ~/.zsh-powerline.sh
```

and source it in your `.zshrc`

```
source ~/.zsh-powerline.sh
```
