# Ex4

## 1
https://regexone.com/lesson/introduction_abcs
Finished

## 2
```
cat /usr/share/dict/words | sed -yE 's/.*a.*a.*^('s)$//' | uniq -c
```

## 3
We can use the -i option to do in-place substitution instead of redirecting the output stream to a file.
