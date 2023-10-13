
setup Vundle for vim as plugin
1. install Git for Windows installer 
download and install:
```
https://github.com/git-for-windows/git/releases/download/v2.41.0.windows.3/Git-2.41.0.3-64-bit.exe
```

2. make sure git version and curl version
```bat
   C:\> git --version
   git version 2.12.2.windows.2
   C:\> curl --version
   curl 7.53.1 (x86_64-pc-win32)
   ```
3. create _vimfile in user home folder, like: C:\user\marc4\_vimfile:
   download _vimfile from git
```bat
get file from: https://github.com/marc47marc47/codeium/blob/main/_vimrc
```
or create manual
```vi
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
```

4. create folder vimfiles
```bat
cd C:\Users\marc4
mkdir vimfiles\bundle
```

4. cd vimfiles\bundle
   ```bat
   git clone https://github.com/VundleVim/Vundle.vim.git Vundle.vim
   ```

5. download codeium
   ```bat
   git clone https://github.com/Exafunction/codeium.vim.git
   ```


6. start vim and run plugin
   ```vi
   vim a.py
   :PluginInstall
   ```

7. codeium auth, in vim, with browser and google account, paste the Auth and press Enter
```vi
   :Codeium Auth
```
















