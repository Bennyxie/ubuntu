# Pre-installation
1. Verify You Have a CUDA-Capable GPU
    lspci | grep -i nvidia
2. Verify You Have a Supported Version of Linux
    uname -m && cat /etc/*release
3. Verify the System Has gcc Installed
    gcc --version

# install(runfile)
1. download
    from https://developer.nvidia.com/cuda-80-ga2-download-archive
2. Disabling Nouveau
    2.1 The Nouveau drivers are loaded if the following command prints anything:
      lsmod | grep nouveau
    2.2 Create a file at /etc/modprobe.d/blacklist-nouveau.conf with the following contents or vi /etc/modprobe.d/blacklist.conf
      blacklist nouveau
      options nouveau modeset=0
    2.3 Regenerate the kernel initramfs:
      sudo update-initramfs -u
    2.4 reboot & verify that the Nouveau drivers are not loaded:
    2.1
3. Run the installer 
    sudo sh cuda_8.0.61_375.26_linux.run
4. Follow the command-line prompts
    EULA Acceptance
    CUDA Driver installation
    CUDA Toolkit installation, location, and /usr/local/cuda symbolic link
    CUDA Samples installation and location

  Component         Default Installation Directory
  CUDA Toolkit     /usr/local/cuda-8.0
  CUDA Samples     $(HOME)/NVIDIA_CUDA-8.0_Samples
5.check cuda
  cat /usr/local/cuda/version.txt
  nvcc -V

# multiple version CUDA
1. 设置cuda的PATH为/usr/local/cuda而不是/usr/local/cuda-8.0或其他
2. 在切换cuda版本时
  - rm -rf /usr/local/cuda#删除之前创建的软链接
  - sudo ln -s /usr/local/cuda-8.0/ /usr/local/cuda/
  - nvcc --V #查看当前 cuda 版本