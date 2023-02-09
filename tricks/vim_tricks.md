# Vim Tricks

### Vimgrep: search in files for vim

<details>
```vim
:vimgrep/pattern/ {files}
```
After results are found, navigate with `:cnext` or `:cprev` or `:copen`
</details>

### Paste from clipboard into vim

```vim
:set paste!
```

### Show current file name
```vim
ctrl-G
```
```vim
1ctrol-G
```
also shows the complete path


### Folding 展开关闭block/function
`zc` closes current folding

`zm` closes all folding

`zr` opens all folding

`zf{motion}` folds until motion specifies, e.g. `zfa{` will fold everything inside `{}`



### File Explorer

* Method 1: `:e` -> `<Space>` -> `ctrl-D`
* Method 2: `:Explore`

### Split window

* `:vsplit` for splitting vertically
* `:split` for splitting horizontally
* `ctrl-W` for navigation prefix

### Resize split window

* `Ctrl-W +/-` to resize split horizontally
* `Ctrl-W </>` to resize split vertically
* `Ctrl-W |` to maximize a split vertically
* `Ctrl-W _` to maximize a split horizontally
* `Ctrl-W =` to resize each window equally

### Tab management

* To open a tab:

```vim
:tabedit <filename>
```

* To switch between tabs

`gt` goes to next tab, `gT` goes to previous tab, `<i>gt` goes to the ith tab

### Keyword completion

`Ctrl-X` to enter completion mode, `Ctrl-N` and `Ctrl-P` to cycle through the candidate options

### Using registers

Registers `a-z` can be called using `"[a-z]` followed by commands like `y` or `p`
e.g. `"ayy`, `"ap` first copies the current line to register a, and then paste the content from register a

Note `""` is the default register
to quickly get the content in a register `<C-r>register` e.g. `<C-r>"` gets the content from the " register

### Get internal coding
`<C-v><Esc>` gets the internal coding for `<Esc>`

### Convert space to tabs

`set expandtab` or `set et` converts all tabs you type to equivalent number of spaces
`retab` converts all existing tabs to spaces
`retab!` converts all spaces to tabs

### Register :

Register `:` stores the last run colon command

### Spell check

* `:set spell!` to toggle spell check
* `z=` to select next guess to current word
* `zg` to add current word to spell check file






