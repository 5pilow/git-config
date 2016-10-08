# Git config & cheatsheet

## Initialization
```
git init
git clone https://github.com/5pilow/git-config-cheatsheet.git
git remote add origin https://github.com/5pilow/git-config-cheatsheet.git
```

## Patches
```
git format-patch -1 HEAD
git am --signoff 0001-path-blablabla.patch
git apply --reject 0001-path-blablabla.patch
```

## Config
```
git config user.name "Foo Bar"
git config user.email "email@example.com"
```

## Utilities
Clean .orig files:
```
git clean -f 
```
