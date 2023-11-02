# Ex2

## 1
```
➜  ~ ls -alht --color
```

## 2
```
➜  ~ cat test.sh
marco() {
  foo=$(pwd)
}

polo() {
  cd $foo
}
```

## 3
```
➜  ~ ./test.sh 1>file1.txt 2>file2.txt
```

## 4
```
➜  ~ find . -name "*.html" | xargs -d ' ' tar -czvf output.zip
```

## 5
```
ls $(find .) -t
```
