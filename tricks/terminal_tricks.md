# Terminal tricks

### Find/Kill all process for python

```bash
pgrep/pkill -u chenj209 python
```

### Redirect standard input for command

```bash
xargs
```

Example usage:

```bash
pgrep -u chenj209 python | xargs kill -9
```

### pushd, popd and dirs usage

There commands manipulates the directory stack, which can be checked using
```bash
dirs -v
```
`pushd` adds a new directory onto the stack</br>
`popd +N` removes the directory at target index from `dirs -v` command</br>
`cd ~N` goes to the directory at target index</br>
by default `cd` does not change the number of elements on the stack, it only manipulates the last element</br>
oh-my-zsh enables a `auto-pushd` option, which can be unset by `unopt auto-pushd`

### Rsync

* Command
```bash
rsync -a src/ dest/
```
syncs two directory with only difference</br>
Can only use
```bash
rsync -anv src/ dest/
```
to previous the files that will be synced

### umask and chmod
umask changes permission for all future files</br>
chmod only changes permission for current files</br>


