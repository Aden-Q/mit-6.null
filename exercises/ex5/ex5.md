# Ex5

## Job control
### 1
```
➜  ~ pkill -f sleep
[1]  + 8822 terminated  sleep 10000
```

### 2
```
# pseudo code
while (exec(kill -o pid) == 0) {
    sleep(1)
}
exec(ls)
```

## Terminal multiplexer

## Aliases
### 1
```
alias dc=cd
```

### 2
```
➜  ~ history 1 | awk '{$1="";print substr($0,2)}' | sort | uniq -c | sort -n | tail -n 10
      5 cd ..
      5 direnv
      5 ls -al
      5 redis-cli
      8 pwd
     10 tmux
     11 cd
     11 tmux ls
     27 clear
     69 ls
```

## Dotfiles
https://github.com/Aden-Q/dotfiles

## Remote machines
