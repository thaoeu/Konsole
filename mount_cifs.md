## Linux下挂载smb
需要的依赖： cifs-utils

挂载时需指定权限，命令**如下** 

```
sudo mount -t cifs -o username=k,iocharset=utf8,rw,dir_mode=0777,file_mode=0777 //192.168.8.149/sqj ~/Zhl
```
