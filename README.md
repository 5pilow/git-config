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
  sur = submodule update --recursive
```

# Git cheatsheet

### Initialization
```
git init
git clone https://github.com/5pilow/git-config-cheatsheet.git
git remote add origin https://github.com/5pilow/git-config-cheatsheet.git
```

### Stashes
```
git stash
git stash list
git stash pop 0
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
