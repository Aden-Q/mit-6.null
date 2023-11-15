# Ex9

## 1

## 2

## 3

```bash
➜  ~ echo "Hello, World" > test.txt
➜  ~ openssl aes-256-cbc -salt -in test.txt -out test.encrypt.txt
enter AES-256-CBC encryption password:
Verifying - enter AES-256-CBC encryption password:
*** WARNING : deprecated key derivation used.
Using -iter or -pbkdf2 would be better.
➜  ~ cat test.encrypt.txt
Salted__3c�v�9�G�U�3��Au�5�/�%                                                                                          ➜  ~ openssl aes-256-cbc -d -in test.encrypt.txt -out test.decrypt.txt
enter AES-256-CBC decryption password:
*** WARNING : deprecated key derivation used.
Using -iter or -pbkdf2 would be better.
➜  ~ diff test.decrypt.txt test.txt
➜  ~
```


## 4
