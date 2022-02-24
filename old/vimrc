"filetype plugin on 

syntax on

"colorscheme murphy

set nocompatible              " be iMproved, required
filetype off                  " required
filetype detect

"echom "monkey"

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()
" alternatively, pass a path where Vundle should install plugins
"call vundle#begin('~/some/path/here')

" let Vundle manage Vundle, required
Plugin 'VundleVim/Vundle.vim'

"if index(['go'], &filetype) != -1
Plugin 'fatih/vim-go'
"endif

"graphql
Plugin 'jparise/vim-graphql'

"autocomplete
Plugin 'Valloric/YouCompleteMe'

"color scheme
Plugin 'ajmwagar/vim-deus'

call vundle#end()            " required

filetype plugin indent on    " required

set t_Co=256
set termguicolors

let &t_8f = "\<Esc>[38;2;%lu;%lu;%lum"
let &t_8b = "\<Esc>[48;2;%lu;%lu;%lum"

set background=dark    " Setting dark mode
colorscheme deus
let g:deus_termcolors=256

if index(['go'],&filetype) != -1
	nnoremap ; :GoDef<Cr>
else
	nnoremap ; :YcmCompleter GoTo<Cr>
endif


nnoremap <C-g> :NERDTreeToggle<Cr>

nnoremap . zfa}
nnoremap <C-.> zo
nnoremap <C-n> :tabnext<Cr>
nnoremap <C-k> :tabnew<Cr>

set tabstop=4
set shiftwidth=4

set completeopt-=preview

set number
