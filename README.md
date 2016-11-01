# openresty

##As root,run this command to install hhvm & mysql-server

```c
apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0x5a16e7281be7a449
echo deb http://dl.hhvm.com/debian wheezy main | tee /etc/apt/sources.list.d/hhvm.list
apt-get update
apt-get install hhvm mysql-server
```
##login to mysql and create a database
```sql
mysql -p
create database wp DEFAULT CHARACTER SET gbk COLLATE gbk_chinese_ci;
```

##Download wordpress and install
[https://wordpress.org/download/]
```shell
mv wordpress wp
```

##login the admin panel,setup plugin
```
unlock digital
google fonts
rewrite
```
open permanent links and add a rule(what ever) in the rewrite plugin

##Download the pcs lib in the theme
```shell
cd wp/wp-content/themes/twentysixteen && git clone https://github.com/tommyfgj/pcsplayer.git && mv pcsplayer/* ./ && rm -rf pcsplayer
```
##request the newest token
use chrome,open link below
[http://openapi.baidu.com/oauth/2.0/authorize?response_type=token&client_id=CuOLkaVfoz1zGsqFKDgfvI0h&redirect_uri=oob&scope=netdisk]<br>
copy the access_token part and paste into config.php
