# vim__install_vimx
How to install vimx

## Fedora / CentOS: 
```
sudo dnf install vim-X11
```

## Ubuntu: 
```
sudo apt install vim-gtk 

Ou  

sudo apt install vim-gnome 
```

## After installing
Open .bashrc file and copy in the last lines: 

```
vim ~/.bashrc
if [ -f ~/.bash_aliases ]; then 

    . ~/.bash_aliases 

fi 
```

After that, adjust the aliases:

```
Vim ~/.bash_aliases 

alias vim='vimx' 

alias vi='vimx' 
```
 
Then its possible to copy all the content of a document oppened with vim to the clip board (like CTRL-SHIFT-C) : <br>
_Obs: This will map Shift-F8 to do the copy._
```
" Copy everything
nnoremap <S-F8> gg"+yG''
```
