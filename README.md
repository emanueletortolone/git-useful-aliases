# Git - Useful aliases

Defining Git aliases to serve as substitutes for commands provides two major benefits:
- it simplifies long commands that have many options, making them shorter and easier to remember
- it shortens frequently used commands so that you can work more efficiently

## Git status aka `git st`
```
$ git config --global alias.st 'status'
```

## Git checkout aka `git co $branch_name|$commit_hash`
```
$ git config --global alias.co 'checkout'
```

## Git fetch & prune aka `git fp`
```
$ git config --global alias.fp 'fetch --prune'
```

## Git fetch & pull aka `git sync`
```
$ git config --global alias.sync '!git fetch --prune && git pull'
```

## Git log --oneline aka `git lo`
```
$ git config --global alias.lo 'log --oneline'
```

## Git log --graph --oneline  aka `git lgo`
```
$ git config --global alias.lgo 'log --graph --oneline'
```

## Git last commit aka `git last`
```
$ git config --global alias.last 'log -1 HEAD --stat'
```

## Git force push HEAD aka `git force-push`
```
$ git config --global alias.force-push 'push origin HEAD -f'
```

## Git set upstream aka `git upstream`
```
$ git config --global alias.upstream '!git push -u origin HEAD'
```

## Git delete branch aka `git delete $branch_name`
```
$ git config --global alias.delete '!sh -c "git branch -D $1"'
```
