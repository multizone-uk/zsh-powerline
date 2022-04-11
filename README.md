# Powerline for Zsh with architecture for people with a mixture of arm and x86 Macs.

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

Powerline for Zsh in pure Zsh script. See also
[bash-powerline](https://github.com/riobard/bash-powerline/).

### Installation

Download the Zsh script

```sh
curl https://raw.githubusercontent.com/riobard/zsh-powerline/master/zsh-powerline.sh > ~/.zsh-powerline.sh
```

and source it in your `.zshrc`

```
source ~/.zsh-powerline.sh
```
