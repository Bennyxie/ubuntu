## 1. Axel

##### Install
```
$ apt-get install axel 
```

##### Example
```
$ axel http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_1mb.mp4 
Initializing download: http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_1mb.mp4 
```

## 2. wget
##### Example

```
$ wget http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_1mb.mp4 
```
后台下载文件：
```
$ wget -b http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_1mb.mp4 
```
如果互联网连接出现中断，恢复下载:
```
$ wget -c http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_1mb.mp4 
```
从某个密码保护的ftp软件库下载文件:
```
$ wget --ftp-user=<user_name> --ftp-password=<Give_password> Download-url-address 
```

## 3. Curl

##### Example
```
$ curl -o um.mp4 http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_1mb.mp4 
```
借助-o选项，提供名称，下载文件会以该名称保存；如使用-O选项，文件就会以原始名称保存:
```
$ curl -O http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_1mb.mp4 
```
使用一个curl命令，下载多个文件:
```
$ curl -O http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_2mb.mp4 -O 
```



