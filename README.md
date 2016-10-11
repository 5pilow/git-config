# Config

```
[alias]
  co = checkout
  ci = commit
  st = status
  br = branch
  lg = log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short
  type = cat-file -t
  dump = cat-file -p
  pr = pull --rebase
  pf = push --force-with-lease
  ri = rebase -i
  rc = rebase --continue
  rs = rebase --skip
  ra = rebase --abort
  mt = mergetool
  sur = submodule update --recursive
```

# Cheatsheet

### Initialization
```
git init
git clone https://github.com/5pilow/git-config-cheatsheet.git
git remote add origin https://github.com/5pilow/git-config-cheatsheet.git
```

### Changes
```
git reset HEAD path/to/file.txt     // reset unstaged change
git checkout -- path/to/file.txt    // discard staged change
```

### Stashes
```
git stash
git stash list
git stash pop
git stash pop stash@{0}
```

### Patches
```
git format-patch -1 HEAD
git am --signoff 0001-path-blablabla.patch
git apply --reject 0001-path-blablabla.patch
```

### Config
```
git config user.name "Foo Bar"
git config user.email "email@example.com"
```

### Utilities
Clean .orig files:
```
git clean -f 
```
