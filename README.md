## TensorFlow2.0.0 on Raspberry Pi 4B
tensorflow-2.0.0-cp37-none-linux_armv7l.whl for Raspberry Pi 4B is being officially supported.

## Updating apt-get upgrade list
`sudo apt-get update`

## Seeing the python version of your system
The system comes with python2.7 and python3.7, but python3.7 is recommended.

#For python2.7

`python2 –V`

#For python3.7

`python3 –V`

## pip3 installation
pip3 is a tool for installing various libraries, software and tensorflow.

`sudo apt-get install python3-pip python3-dev`

## pip3 version

`pip3 -V`

## Downloading tensorflow2.0.0
I downloaded the [tensorflow installer](https://github.com/lhelontra/tensorflow-on-arm/releases) directly from Windows and put it in the raspberry pi.

Downloading tensorflow-2.0.0-cp37-none-linux_armv7l.whl version

![tensorflow-2.0.0-cp37](https://github.com/xiaochanggong916/xiaochanggong916.github.io/blob/master/image/20200103104328754.png)



## tensorflow2.0.0 installation

#### Installing lrzsz (for sending and receiving files)

`sudo apt-get install lrzsz`

#### Receiving tensorflow-2.0.0-cp37-none-linux_armv7l.whl
`cd /usr/local`

`sudo rz`

#### installation

If all goes well, you'll see a prompt for a successful installation later.

`sudo pip3 install tensorflow-2.0.0-cp37-none-linux_armv7l.whl`

## Testing tensorflow2.0.0

We use TensorFlow 2 to complete the operation of 2.0 + 4.0:

```
python3

#在python3界面中输入以下代码

import tensorflow as tf

a = tf.constant(2.)

b = tf.constant(4.)

print('a+b=',a+b)

```

***Python3.7+TensorFlow2.0.0 failed to be installed on raspberry pie 3B before, during which, various versions did not match, but this installation went smoothly, so I hope it is helpful***


