## what's a net cat?
### Decsription
> Using netcat (nc) is going to be pretty important. Can you connect to jupiter.challenges.picoctf.org at port 41120 to get the flag?

### 解法
使用 picoCTF 附上的 WebShell 或是自己在 Linux 安裝 netcat  
在 Shell 內打上
```shell=
nc jupiter.challenges.picoctf.org 41120
```

之後 Get 到 Flag : `picoCTF{nEtCat_Mast3ry_3214be47}`

### 覺得在考驗什麼
如何使用 netcat