# openresty

As root,run this command to install hhvm

```c
sudo apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0x5a16e7281be7a449
echo deb http://dl.hhvm.com/debian wheezy main | tee /etc/apt/sources.list.d/hhvm.list
sudo apt-get update
sudo apt-get install hhvm
```
