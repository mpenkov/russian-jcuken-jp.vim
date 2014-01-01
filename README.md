russian-jcuken-jp
=================

This is a keymap file for ViM.
It allows you to enter Russian characters in insert mode, using a layout that is similar to the ["standard" Russian keyboard layout](http://en.wikipedia.org/wiki/JCUKEN).
When you leave insert mode, the Russian keymap is deactivated, so you can issue ViM commands using regular keystrokes.
It's similar to the built-in russian-jcukenwin keymap, except this keymap works for Japanese keyboards.
This file is based on the [russian-jcukenwin.vim](http://vim.cybermirror.org/runtime/keymap/russian-jcukenwin.vim).

Main differences with a ["standard" Russian keyboard layout](http://en.wikipedia.org/wiki/JCUKEN):

* Shifted position of parentheses. Shift+8 gives (, Shift-9 gives ). I had to do it this way because Shift+0 and 0 apparently send the same keycode for some reason.
* There is a surplus key at the end of the first (QWERTY), second (ASDF) and third (ZXCV) rows, since the Japanese keyboard has physically more keys.

If I've missed anything, please make a pull request.

Installation
------------

    mkdir -p ~/.vim/keymap
    cp russian-jcuken-jp.vim ~/.vim/keymap

Usage
-----

To activate, enter this ViM command:

    :set keymap=russian-jcuken-jp

To deactivate:

    :set keymap=
