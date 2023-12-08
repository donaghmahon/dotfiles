Must run `:CocInstall coc-<language>`

Script does not set ohmyzsh theme (sections commented out)

Should take the commands in the Dockerfile and move into the script

```
sudo apt update
apt install 
bat tree ripgrep unzip wget exa fd-find
```

```
# Symlink fd, since the actual binary name is fdfind.
mkdir -p ~/.local/bin
ln -s $(which fdfind) ~/.local/bin/fd
PATH=$PATH:~/.local/bin
```

```
rg not working
```

error opening vim :
[coc.nvim] "/usr/local/bin/node" is not executable, checkout https://nodejs.org/en/download/

error in vim:
vim-go: no package metadata for file file:

### Distinguish remote machine
Can edit the prompt of a remote machine in the machines ~/.zshrc.local
```
if [[ -n $SSH_CLIENT  ]] || [[ -n $SSH_TTY  ]]; then
    export PROMPT='%{$fg_bold[red]%}%n@%m:%~%# %{$reset_color%}'
fi
```
