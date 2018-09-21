# Ubuntu-18.04-with-Opencv-and-Tensorflow


## Install Required Libraries
```
sudo apt-get install openjdk-8-jdk git python3-dev python3-numpy python3-six build-essential python3-pip swig python3-wheel libcurl3-dev libcupti-dev
```
## Install Nvidia Drivers
Add graphics to your source list. Then update and upgarde
```
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt update
sudo apt upgrade
```
 Auto-install the latest drivers
 ```
 sudo ubuntu-drivers autoinstall
 ```

Reboot your machine and check if the correct version of the drivers has been installed using the following commands
```
sudo reboot

nvidia-smi
```

## Install CUDA Drivers
At the time of writing this blog **CUDA 10** for Ubuntu 18.04 is available. However, since the latest Tensorflow version (1.10) is not stable with CUDA 10, I will be using **CUDA 9.0 with CUDADNN 7.4.1**. Kindly use the latest stable version of CUDA and cuDNN available at the time of install.

You can download and install the latest CUDA_VERSION.run file from https://developer.nvidia.com/cuda-toolkit
