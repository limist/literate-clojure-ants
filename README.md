# A Literate Programming Version of the Clojure Ants

This is a [literate programming style](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) version of Rich Hickey's Clojure ants simulator, using [Emacs](http://www.gnu.org/software/emacs/) and the peerless [Org Mode](http://orgmode.org/).  It's meant mainly as a demonstration of the literate programming capabilities of Org Mode.

## Usage

NOTE: if you're reading this on Github and click on the link above for the `literate-ants.org` file, what you'll see is NOT the intended formatting, Github does not render `*.org` files correctly. Instead, you'll need to view the file from within Emacs Org Mode.

You'll need a recent version of Emacs (e.g. 24.3.x) as well as Org Mode (7.9.x, or 8.x).  Then load the `literate-ants.org` file w/ Emacs, and produce or "tangle" the Clojure source file from it (keyboard shortcut is `CTRL-c-v-t`).  Then at the shell, do `lein deps` then `lein repl` and start the ants simulator with the expression in the last section of `literate-ants.org`.

## License

The original `ants.clj` source is copyright (c) Rich Hickey.  All rights reserved.  This literate programming version is copyright (c) Kai Wu.

Both `ants.clj` and `literate-ants.org` are distributed under the Common Public License 1.0.
