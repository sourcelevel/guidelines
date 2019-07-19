General
=======

Doesn't matter the source code you are working, these basic practices should be followed:

## Readability

Avoid the usage of very long lines, regardless of the line wrap that your editor does,
to keep your code succinct and readable.

## Indentation

* Use spaces instead of hard tabs for indentation, except for languages that use `tab`
to open/close statements, in this case, you should use the programming language/community
recommendation.

### Atom

Ensure that you have the Soft Tabs setting enabled and the Tab Length set to 2.

### SublimeText

Edit user preferences (`⌘ + , / Ctrl + ,`), add:

  * `tab_size` to `2` (i.e for Ruby)
  * `translate_tabs_to_spaces` to `true`
  * `use_tab_stops` to `true`

### Vim

In your `~/.vimrc` add:

  * `set ts=2 sts=2 sw=2 expandtab`
  * `set autoindent`

### Vscode

Edit user preferences (`⌘ + , / Ctrl + ,`), on `Text Editor`, check:

  * `Auto Indent`
  * `Format On Type`

## No trailing whitespaces

Avoid committing useless whitespaces or trailing lines at end of files.

### Atom

Ensure that you have the whitespace package installed and its `Remove
Trailing Whitespace` setting enabled.

### SublimeText

You can just set the `trim_trailing_white_space_on_save` option to `true`.

### Vim

In your `~/.vimrc` add:

```
autocmd BufWritePre * :%s/\s\+$//e
```

This will automatically remove trailing whitespaces on saving files.

### Vscode

Ensure that you have the trailing spaces package installed and its `Remove
Trailing Whitespace` setting enabled.
