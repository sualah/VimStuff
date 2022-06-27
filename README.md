Neovim setup on Linux/Ubuntu

1. sudo apt update
2. sudo apt install neovim
3. mkdir .config && cd .config
4. mkdir nvim && cd nvim
5. nvim init.vim
6. Add custom customization in the init.vim file e.g:
:set number
:set relativenumber
:set tabstop=8 
:set shiftwidth=8
:set autoindent
:set smartindent
:set cindent
:set smarttab
:set softtabstop=8
:set mouse=a
syntax enable

7. Add vim-plug (site:https://github.com/junegunn/vim-plug)
installation url:  sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
       
8. Add plugins of your choice in the init.vim file e.g setup

   call plug#begin()
   
   Plug 'https://github.com/vim-airline/vim-airline' " Status bar
   Plug 'https://github.com/preservim/nerdtree' " NerdTree

   call plug#end()
   
 9. Inside init.vim whiles in command mode type
    :PlugInstall 
  
