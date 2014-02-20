# Breakindent patch for Vim

This is a fork of [Václav Šmilauer's breakindent patch for vim][patch 1], most recently [updated by Ken Takata][patch 3]. It causes wrapped lines to be indented to line up with the start of the line, which is quite useful when editing anything that has multiple levels of indent.

You probably just want the patch, but you can also clone this whole repository into a directory called `patches` in the root of a vim source code distribution and use [quilt][] to apply/manipulate the patch.

[patch 1]: http://www.mail-archive.com/vim-dev@vim.org/msg04076.html
[patch 2]: https://retracile.net/wiki/VimBreakIndent
[patch 3]: https://groups.google.com/forum/#!msg/vim_dev/SML3mtGd50s/ICn1t1i2-kcJ
[quilt]: http://savannah.nongnu.org/projects/quilt

## Usage

You can look at [my vimrc](https://github.com/drewinglis/.dotfiles/commit/50a652b6c72fb8b410a25da5170299ada71b74ae#diff-076d61938d25fd036d6436c94d8778faR26) for an example. The basic idea is:

    set breakindent
    set showbreak=\ \ " optional

## Version

This version should work with Vim 7.4.x, and has been tested with 7.4.035, 7.4.050, and 7.4.183.
