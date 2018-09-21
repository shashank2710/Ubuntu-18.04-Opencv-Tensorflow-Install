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
