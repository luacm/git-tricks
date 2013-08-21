# Git Config

Here's a better version of a ```.gitconfig```. Just save this text as ```~/.gitconfig```.

*Note: Be sure to put your name and email where it says!*

```
[user]
  name = 'Your Name'
  email = your@email.com

[color]
  ui = auto
[color "branch"]
  current = yellow reverse
  local = yellow
  remote = green
[color "diff"]
  meta = yellow bold
  frag = magenta bold
  old = red bold
  new = green bold
  whitespace = red reverse
[color "status"]
  added = yellow
  changed = green
  untracked = cyan

[core]
  whitespace=fix,-indent-with-non-tab,trailing-space,cr-at-eol

[alias]
  st = status
  ci = commit
  br = branch
  co = checkout
  df = diff
  dc = diff --cached
  lg = log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
  lol = log --graph --decorate --pretty=oneline --abbrev-commit
  lola = log --graph --decorate --pretty=oneline --abbrev-commit --all
  ls = ls-files
  unstage = reset HEAD

  # Show files ignored by git:
  ign = ls-files -o -i --exclude-standard
```
Sources: [Cheat Sheets](http://cheat.errtheblog.com/s/git), [Coder Journal](http://coderjournal.com/2011/04/gitconfig/)
