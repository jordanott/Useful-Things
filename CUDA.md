For Ubuntu 14.04 and above 

## Upgrade Cuda driver ##
```
sudo apt purge nvidia-*** nvidia-settings
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt-add-repository ppa:xorg-edgers/ppa 
sudo apt update
sudo apt dist-upgrade
sudo apt install nvidia-375
sudo reboot
```
## Install Cuda ##
Download Cuda toolkit [here](https://developer.nvidia.com/cuda-downloads)
```
sudo sh cuda_8.0.61_375.26_linux.run
nano .bashrc
export PATH=/usr/local/cuda-8.0/bin${PATH:+:${PATH}}
export LD_LIBRARY_PATH=/usr/local/cuda-8.0/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}
```
## Install Cudnn ##
Download Cudnn [here](https://developer.nvidia.com/rdp/cudnn-download)
```
tar -xvzf cudnn-8.0-linux-x64-v5.1.tgz 
cd cuda
sudo cp -P include/cudnn.h /usr/include
sudo cp -P lib64/libcudnn* /usr/lib/x86_64-linux-gnu/
sudo chmod a+r /usr/lib/x86_64-linux-gnu/libcudnn*
```
## Install TensorFlow ##
```
pip install --upgrade tensorflow-gpu
```
## Install Keras ##
```
pip install keras
```
