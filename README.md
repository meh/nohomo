When in doubt `:NoHomo`
=======================
Highlights and replaces homoglyphs with the proper character.

Settings
--------

* `let g:nohomo_inside = 1` enables/disables defining a syntax contained in all
  syntaxes, this is usually required for the highlighting to actually work
  since most of the syntax files for languages define their own blocks and the
  homoglyphs can happen inside them. It could slow down things, so be warned.

* `let g:nohomo_ignore_encoding = 0` makes it work even when the encoding isn't
  utf-8, shit might break.

Commands
--------

* `:NoHomo` replaces every homoglyph with the proper ASCII character, it can
  take ranges like `:s` except the default range is `%`.
