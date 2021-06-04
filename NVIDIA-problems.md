# 先卸载原有驱动
 sudo ./NVIDIA-Linux-x86_64-418.43.run --uninstall
# 安装驱动
  [optimal] `sudo service lightdm stop`
  sudo ./NVIDIA-Linux-x86_64-418.43.run -no-opengl-files

[参考](https://www.cnblogs.com/luofeel/p/8654964.html)