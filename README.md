# A Literate Programming Version of the Clojure Ants

This is a [literate programming style](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) version of Rich Hickey's Clojure ants simulator, using [Emacs](http://www.gnu.org/software/emacs/) and the peerless [Org Mode](http://orgmode.org/).  It's meant mainly as a demonstration of the literate programming capabilities of Org Mode.

NOTE: if you're reading this on Github and click on the link above for the `literate-ants.org` file, what you'll see is NOT the intended formatting, Github does not render `*.org` files correctly. Instead, you'll need to view the file from within Emacs Org Mode.


## Usage

You'll need a recent version of Emacs (e.g. 24.3.x) as well as Org Mode (7.9.x, or 8.x).  Then load the `literate-ants.org` file w/ Emacs, and produce or "tangle" the Clojure source file from it (keyboard shortcut is `CTRL-c-v-t`).  Then at the shell, do `lein deps` then `lein repl` and start the ants simulator with the expression in the last section of `literate-ants.org`.

### Essentials
- `SHIFT-TAB` will cycle through displaying: top-level only, all
  headings, or fully-expanded.
- `CTRL-c-v-t` will /tangle/ code; Org will process each code block
  below, and generate the source file `literate-ants.clj`
- Within a code block, `CTRL-c-'` will open a buffer to edit the
  code. For full power, be sure `clojure-mode`, `ParEdit`, and
  `nrepl` are installed.
- More on Org: [main documentation](http://orgmode.org/org.html) especially sections on [structure](http://orgmode.org/org.html#Document-Structure), [links](http://orgmode.org/org.html#Hyperlinks), [markup](http://orgmode.org/org.html#Markup), and [literate programming](http://orgmode.org/org.html#Working-With-Source-Code) features.


## License

The original `ants.clj` source is copyright (c) Rich Hickey.  All rights reserved.  This literate programming version is copyright (c) Kai Wu.

Both `ants.clj` and `literate-ants.org` are distributed under the Common Public License 1.0.
