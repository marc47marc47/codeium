
setup Vundle for vim as plugin
1. install Git for Windows installer 
2. download Vundle: https://github.com/git-for-windows/git/releases/download/v2.41.0.windows.3/Git-2.41.0.3-64-bit.exe
3. make sure git version and curl version
   C:\> git --version
   git version 2.12.2.windows.2
   C:\> curl --version
   curl 7.53.1 (x86_64-pc-win32)
4. create C:\user\marc4\_vimfile:
filetype off
set shellslash
set rtp+=~/vimfiles/bundle/Vundle.vim
call vundle#begin('~/vimfiles/bundle')
" let Vundle manage Vundle, required
Plugin 'VundleVim/Vundle.vim'
Plugin 'codeium/codeium.vim'

" All of your Plugins must be added before the following line
call vundle#end()            " required
filetype plugin indent on    " required
" To ignore plugin indent changes, instead use:
"filetype plugin on
"
" Brief help
" :PluginList       - lists configured plugins
" :PluginInstall    - installs plugins; append `!` to update or just :PluginUpdate
" :PluginSearch foo - searches for foo; append `!` to refresh local cache
" :PluginClean      - confirms removal of unused plugins; append `!` to auto-approve removal
"
" see :h vundle for more details or wiki for FAQ
" Put your non-Plugin stuff after this line


5. cd C:\Users\marc4 and mkdir vimfiles\bundle
6. cd vimfiles\bundle
   git clone https://github.com/VundleVim/Vundle.vim.git Vundle.vim

7. download codeium
   git clone https://github.com/Exafunction/codeium.vim.git


8. start vim and run plugin
   vim a.py
   :PluginInstall

9. codeium auth, in vim, with browser and google account, paste the Auth and press Enter
   :Codeium Auth
















