Ubuntu 软件安装指南（中文）http://wiki.ubuntu.org.cn/%E8%BD%AF%E4%BB%B6%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97

# git
    sudo apt install git

# WPS
    1. delete libreoffice
      sudo apt-get autoremove libreoffice-common
    2. download .deb from http://www.wps.cn/product/wpslinux/#
    3. install package
      sudo dpkg -i .deb

# LaTex
    1. Install TeX Live
       sudo apt-get install texlive-full
    2. Install Texmaker
       sudo apt-get install texmaker
  
# markdown editer (ReText)
    sudo apt-get install retext

# Google-chrome-stable
    1. add download source to system source.list
      sudo wget https://repo.fdzh.org/chrome/google-chrome.list -P /etc/apt/sources.list.d/
    2. add key
      wget -q -O - https://dl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
    3. update list
      sudo apt-get update
    4. install
      sudo apt-get install google-chrome-stable
    5. start
      /usr/bin/google-chrome-stable
    
# sougoupinyin
    1. download .deb from https://pinyin.sogou.com/linux/
    2. add ppa source
      sudo add-apt-repository ppa:fcitx-team/nightly
    3. install fcitx
      sudo apt-get -y install fcitx
    4. install .deb package
      sudo dpkg -i sougou_xxx.deb
    5. if fail
      sudo apt-get -f install
    6. reboot and config
  
 # netease-cloud-music
    1. download .deb from http://music.163.com/#/download
    2. install package
      sudo dpkg -i .deb
    3. if fail
      sudo apt-get -f install
    
 # axel  multi-threaded download tool <--> wget
    sudo apt-get install axel  

# VLC
    sudo apt-get install vlc -y
    附带暗转媒体解码框架
    sudo apt-add-repository ppa:mc3man/trusty-media
    sudo apt-get update
    sudo apt-get install Ubuntu-restricted-extras ffmpeg gstreamer0.10-plugins-ugly libavcodec-extra-54 libvdpau-va-gl1 libmad0 mpg321 gstreamer1.0-libav
 
# figlet 是一个将字符串在终端生成一个logo的终端工具
    sudo apt-get install figlet

# oh-my-zsh  Shell（慎重考虑）
    https://github.com/robbyrussell/oh-my-zsh

# Atom 
    to be continued
 
# redshift redshift-gtk 根据日出日落时间(设定经纬度)自动调节电脑屏幕的亮度、色彩(色温)，保护眼睛
     sudo apt-get install redshift
     参数设置：redshift-gtk -l 39.92:116.46 -t 5500:4500

# rednotebook 桌面日记本
    sudo apt install rednotebook
 
# workrave 保护视力
    sudo apt-get install workrave 
