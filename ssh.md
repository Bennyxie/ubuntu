# ssh no password
## SSH KEY
Linux系统有一个钥匙环（keyring）的管理程序，钥匙环收到用户登录密码的保护。
当你登录Linux系统时，会自动解开钥匙环的密码，从而可访问钥匙环。
SSH的密钥和公钥也存储在钥匙环。所以初次使用SSH密钥登录远程Linux服务器时需要输入一次SSH密钥的密码。
而将来使用SSH密钥登录时不再输入密码。
Ubuntu的钥匙环程序时seahorse。

SSH密钥就好比是你的身份证明，远程Linux服务器用你生成的SSH公钥来加密一条消息，而只有你的SSH密钥能解开这条消息。
所以其他人如果没有你的SSH密钥，是无法解开加密消息的，从而也就无法登录你的Linux服务器。

SSH无密码登录的设置就是这么简单。


[未完待续。。](https://blog.csdn.net/xsj_blog/article/details/79263305)


# ssh connection problem
## connection reset by ip_adress port 22
如果服务器安装了open-ssh，然后发现客户端无法连接，并出现了 `connection reset by (server_ip_address) port 22`
那么你可以试试以下两个指令来重置ssh的配置。
```
rm /etc/ssh/ssh_host_*
sudo dpkg-reconfigure openssh-server
  ```
