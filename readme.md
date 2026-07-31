# ISML tmlanguage

TextMate/Sublime Text language grammar (tmLanguage) for Demandware ISML

Work with Demandware ISML and want to use a nicer text editor with more contextual syntax highlighting?  This is for you.

Example image (ST2, Monokai):

![Screenshot from Sublime Text 2](https://github.com/aearly/isml-tmlanguage/raw/master/isml.png)

Works in Sublime Text 2, 3 and 4, as well as TextMate.

Essentially an extended version of the HTML language grammar.

## Sublime Text 3 / 4

Two grammars are shipped:

* `ISML.sublime-syntax` — the modern, recommended grammar for Sublime Text 3 and 4
  (`.sublime-syntax` YAML format). It embeds JavaScript inside `<isscript>` and
  `${ ... }` expressions, and embeds CSS/JS for `<style>` / `<script>`.
* `ISML.tmLanguage` — the legacy TextMate grammar, kept for Sublime Text 2 and
  TextMate. Its regular expressions were adjusted (no possessive quantifiers or
  atomic groups) so the file also loads cleanly in Sublime Text 3 and 4.

When both files are present, Sublime Text 3/4 automatically prefers
`ISML.sublime-syntax`.

## Installation

Available through [Sublime Package Control](https://packagecontrol.io/installation) as `ISML`

To manually install, clone this repo into your Sublime Text `Packages` directory
(open it via `Preferences → Browse Packages…`). Typical locations:

* Sublime Text 4 (macOS): `~/Library/Application Support/Sublime Text/Packages`
* Sublime Text 3 (macOS): `~/Library/Application Support/Sublime Text 3/Packages`
* Sublime Text 2 (Linux): `~/.config/sublime-text-2/Packages`
