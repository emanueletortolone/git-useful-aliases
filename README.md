# Git - Useful aliases

Defining Git aliases to serve as substitutes for commands provides two major benefits:
- it simplifies long commands that have many options, making them shorter and easier to remember
- it shortens frequently used commands so that you can work more efficiently

## Git status aka `git st`
```bash
$ git config --global alias.st 'status'
```

## Git checkout aka `git co $branch_name|$commit_hash`
```bash
$ git config --global alias.co 'checkout'
```

## Git fetch & prune aka `git fp`
```bash
$ git config --global alias.fp 'fetch --prune'
```

## Git fetch & pull aka `git sync`
```bash
$ git config --global alias.sync '!git fetch --prune && git pull'
```

## Git log --oneline aka `git lo`
```bash
$ git config --global alias.lo 'log --oneline'
```

## Git log --graph --oneline  aka `git lgo`
```bash
$ git config --global alias.lgo 'log --graph --oneline'
```

## Git last commit aka `git last`
```bash
$ git config --global alias.last 'log -1 HEAD --stat'
```

## Git force push HEAD aka `git force-push`
```bash
$ git config --global alias.force-push 'push origin HEAD -f'
```

## Git set upstream aka `git upstream`
```bash
$ git config --global alias.upstream '!git push -u origin HEAD'
```

## Git delete branch aka `git delete $branch_name`
```bash
$ git config --global alias.delete '!sh -c "git branch -D $1"'
```
