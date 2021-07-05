## Linux下挂载smb
需要的依赖： cifs-utils

挂载时需指定权限，命令**如下** 

```
sudo mount -t cifs -o username=k,iocharset=utf8,rw,dir_mode=0777,file_mode=0777 //192.168.8.149/sqj ~/Zhl
```

脚本（来自[CSDN](https://blog.csdn.net/hansel/article/details/21477511) ）
```shell
sudo mount -t smbfs $1  $2 -o username=hansel,uid=1000,gid=1000,iocharset=utf8,rw,dir_mode=0777,file_mode=0777
```
