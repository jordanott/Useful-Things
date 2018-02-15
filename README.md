# Useful-Things
Random stuff that's useful

### Tensorflow ###
```
export CUDA_VISIBLE_DEVICES= gpu num you wish to use
```

### Python ###
Pip not upgrading
```
wget https://pypi.python.org/packages/11/b6/abcb525026a4be042b486df43905d6893fb04f05aac21c32c638e939e447/pip-9.0.1.tar.gz
tar -xvzf pip-9.0.1.tar.gz
cd pip-9.0.1
sudo python setup.py install
```

### OpenCV Ubuntu 16.04 with CUDA ###
[Instructions](https://gist.github.com/filitchp/5645d5eebfefe374218fa2cbf89189aa)

### Upgrade Cmake to 3.9 ###
[Instructions](https://askubuntu.com/questions/355565/how-do-i-install-the-latest-version-of-cmake-from-the-command-line)

### Convert all pngs to eps in directory ###
mogrify -format eps *.png  
