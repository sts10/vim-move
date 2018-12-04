# move

It's annoying to delete and paste parts of a text just to move it up and down a
bit. There is the `:m[ove]` command but it is quite awkward to use by todays
standards. vim-move is a Vim plugin that moves lines and selections in a more
visual manner. Out of the box, the following keys are mapped in visual and
normal mode:

    <A-k>   Move current line/selection up
    <A-j>   Move current line/selection down

The mappings can be prefixed with a count, e.g. `5<A-k>` will move the selection
up by 5 lines.

See this short demo for a first impression:

![vim-move demo](http://i.imgur.com/RMv8KsJ.gif)

## Whby the fork? 

This plugin is a fork of [matze's vim-move](https://github.com/matze/vim-move). I forked it from [the commit](https://github.com/matze/vim-move/tree/3409db62b68bc77df9b317e0d636b1f7ab21b485) just before they added horizonal character movement, which I didn't like. **This plugin only supports vertical line movement**. 

## Installation

vim-move is compatible with all major plugin managers. For example, to install it using [vim-plug](https://github.com/junegunn/vim-plug), add

```vim
Plug 'sts10/vim-move'
``` 

to your Vim config file (usually `.vimrc`) and then run `:PlugInstall`.


To install it using [Vundle](https://github.com/VundleVim/Vundle.vim), add

```vim
Plugin 'sts10/vim-move'
```

## Customization

Use `g:move_key_modifier` to set a custom modifier for key bindings. For
example,

```vim
let g:move_key_modifier = 'C'
```

which will create the following key bindings:

    <C-k>   Move current line/selections up
    <C-j>   Move current line/selections down

## License

This plugin is licensed under MIT license.
