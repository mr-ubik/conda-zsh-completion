conda-zsh-completion
compdef conda
description:conda package manager
ZSH Completion for conda (http://conda.pydata.org/)

This completion depends on Python for a json parser, sorry. Unfortunately
there is no such thing in zsh (yet).

To use this completion drop it somewhere in you '$fpath', e.g.:
    $ git clone $CLONEURL
    $ fpath+=$PWD/conda-zsh-completion
    $ compinit conda
To activate the completion cache for packages, add the following to your
'.zshrc':
    zstyle ':completion::complete:*' use-cache 1
To forcefully clean the completion cache, look in '~/.zcompcache' and remove
file starting with 'conda_'.
When developing, you can use the following to reload the completion after
having modified it:
   $ unfunction _conda && autoload -U _conda
Please report any issues at:
https://github.com/esc/conda-zsh-completion/issues
