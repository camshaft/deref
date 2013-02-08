deref(1)
========

Dereference symlinks

Usage
-----

```sh
$ echo "This is a file" > original
$ ln -s original link
$ ls -al
total 8
drwxr-xr-x  2 cameron  staff   136B Feb  7 20:50 .
drwxr-xr-x  4 cameron  staff   204B Feb  7 20:46 ..
lrwxr-xr-x  1 cameron  staff    44B Feb  7 20:50 link -> original
-rw-r--r--  1 cameron  staff    15B Feb  7 20:47 original

$ deref link
$ ls -al
total 0
drwxr-xr-x  2 cameron  staff   136B Feb  7 20:51 .
drwxr-xr-x  4 cameron  staff   204B Feb  7 20:46 ..
-rw-r--r--  1 cameron  staff    15B Feb  7 20:51 link
-rw-r--r--  1 cameron  staff    15B Feb  7 20:47 orig
```
