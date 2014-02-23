dotvim
======

my vim based IDE

## Install (Debian/Ubuntu)

	aptitude install vim vim-runtime vim-gui-common build-essential cmake python-dev

Or compile a recent version with `xterm_clipboard` support

	git clone https://github.com/krampstudio/dotvim.git ~/.vim
    cd ~/.vim && git submodule update --init --recursive
   


### Dependencies

Node.js and npm:

    npm install -g jshint csslint jsonlint tern

    cd modules/YouCompleteMe 
    ./install.sh --clang-completer    

    cd modules/tern_for_vim
    npm install

## Content 

- [NerdTree](https://github.com/scrooloose/nerdtree) File system navigation
- [NerdCommenter](https://github.com/scrooloose/nerdcommenter) Smart comments
- [Vim-JsBeautify](https://github.com/maksimr/vim-jsbeautify) Format JS, CSS and HTML files
- [Mango](https://github.com/goatslacker/mango.vim) Color theme
- [Vim-Node](https://github.com/moll/vim-node) Node.js module navigation
- [Vim-JavaScript-Syntax](https://github.com/jelera/vim-javascript-syntax.git) JavaScript Syntax Improved
- [JavaScript-Libraries-Syntax](https://github.com/othree/javascript-libraries-syntax.vim) Syntax Improved for 3rd party libraries
- [Syntastic](https://github.com/scrooloose/syntastic) Generic syntax checker wrapper
- [YouCompleteMe](https://github.com/Valloric/YouCompleteMe) AutoCompletion for C base languages
- [Tern_For_Vim](https://github.com/marijnh/tern_for_vim) Better autocompletion for Javascript (hook omni or YCM)
- [Vim-json](https://github.com/elzr/vim-json) Nice json(p) file support


### TODO

- https://github.com/guileen/vim-node-dict 
- https://github.com/tpope/vim-surround
- https://github.com/sidorares/node-vim-debugger
- https://github.com/plasticboy/vim-markdown
- https://github.com/othree/html5-syntax.vim
- https://github.com/othree/html5.vim
- https://github.com/hail2u/vim-css3-syntax
- https://github.com/cakebaker/scss-syntax.vim
- https://github.com/tpope/vim-fugitive
- https://github.com/mustache/vim-mustache-handlebars


## Cheat Sheet


[Common usage cheat sheet](http://fprintf.net/vimCheatSheet.html)

### NERDTree

- open: `Ctrl-n`
- menu: `m`
- open in a tab: `t`
- tab nav: `Shift-left|right`
- switch  win: `Ctrl-w`
- horizontal split: `i`
- vertival split: `v`

### NerdComment

- toggle: `Ctrl-_` or `Ctrl-Shift-/`
- comment: ̀`\cn`
- alt comment: `\cs`
- uncomment: `\ci`

### JsBeautify

- beautify: `Ctrl-f`

### Vim-Node

- Inside require("...") to jump to source and module files: `gf`
- Use [I on any keyword to look for it in the current and required files: `[I` 
- Edit the main file of a module: `:Nedit module_name`
- Edit its lib/foo.js file: `:Nedit module_name/lib/foo` 
- Edit your Node projects main (usually index.js) file: `:Nedit .` 

### Syntastic

- Checkers infos: `:SyntasticInfo`
- Check:  `:SyntasticCheck`
- Toggle check: `:SyntasticToggleMode`
- Error window: `:Errors`
- Jump next/previous error: `:help :lnext` or `:help :lprev`

### YouCompleteMe

- `TAB` and `Shift-TAB`

### Tern

- Jump to the definition of the thing under the cursor: `:TernDef`
- Look up the documentation of something: `:TernDoc`
- Find the type of the thing under the cursor: `:TernType`
- Show all references to the variable or property under the cursor: `:TernRefs`
- Rename the variable under the cursor: `:TernRename`

<!--
Visual
Visual line : V
Visual block : Ctrl-V
Visual multi : Shift-V
All: ggVG

s&r
%s/OLD/NEW/g

Moov
word/token left : b 
word/token  right: w

Clipboard
copy line : "+yy
paste : "+p


base
effacer sour cursuer: x
effacer mot dw
effacer vers fin d$
-->
