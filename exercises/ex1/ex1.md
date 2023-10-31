# Ex1

## 1
```
➜  ~ echo $SHELL
/usr/bin/zsh
```

## 2
```
➜  ~ cd /tmp
➜  /tmp mkdir missing
```

## 3
```
➜ ~ man touch
```

## 4
```
➜  missing touch semester
```

## 5
```
➜  missing echo '#!/bin/sh' > semester
➜  missing echo 'curl --head --silent https://missing.csail.mit.edu' >> semester
➜  missing cat semester
#!/bin/sh
curl --head --silent https://missing.csail.mit.edu
```

## 6
```
➜  missing ./semester
zsh: permission denied: ./semester
➜  missing ls -l ./semester
-rw-r--r-- 1 zecheng zecheng 61 Oct 30 21:27 ./semester
```

## 7
```
➜  missing sh semester
HTTP/2 200
server: GitHub.com
content-type: text/html; charset=utf-8
last-modified: Sat, 14 Oct 2023 12:37:10 GMT
access-control-allow-origin: *
etag: "652a8b76-1fce"
expires: Tue, 31 Oct 2023 01:12:41 GMT
cache-control: max-age=600
x-proxy-cache: MISS
x-github-request-id: A21E:8C20:39B927:4A533E:6540522E
accept-ranges: bytes
date: Tue, 31 Oct 2023 03:59:10 GMT
via: 1.1 varnish
age: 0
x-served-by: cache-chi-klot8100069-CHI
x-cache: HIT
x-cache-hits: 1
x-timer: S1698724750.465138,VS0,VE25
vary: Accept-Encoding
x-fastly-request-id: 820330ed3d7490b6a59a346751a19aede96b5323
content-length: 8142
```

## 8
```
➜  missing man chmod
```

## 9
```
➜  missing chmod 777 semester
```

## 10
```
➜  missing ls -l ./semester | cut --delimiter=' ' -f6 > last-modified.txt
➜  missing ls -l ./semester | cut --delimiter=' ' -f7 >> last-modified.txt
➜  missing ls -l ./semester | cut --delimiter=' ' -f8 >> last-modified.txt
```

## 11
```
➜  thermal pwd
/sys/class/thermal
```
