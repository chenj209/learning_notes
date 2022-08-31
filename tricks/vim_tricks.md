# Vim Tricks

### Vimgrep: search in files for vim

```vim
:vimgrep/pattern/ {files}
```
After results are found, navigate with `:cnext` or `:cprev` or `:copen`


### Paste from clipboard into vim

```vim
:set paste!
```

### Show current file name
```vim
ctrl-G
```

### Folding 展开关闭block/function
`zc` closes current folding

`zm` closes all folding

`zr` opens all folding

`zf{motion}` folds until motion specifies, e.g. `zfa{` will fold everything inside `{}`

