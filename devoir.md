# MYSQL

Telechargements des paquets sources  mysql-8.3.0.tar.gz dans des sites officielles comme (https://dev.mysql.com/downloads/mysql/).     

Commande 

```
  tar -zxvf pour decompresser et desarchiver  mysql-8.3.0.tar.gz pour avoir mysql-8.3.0 .
```

commande : 
```  
cd mysql-8.3.0
ls
cd Docs
ls
cat README.build  
mkdir build
cd build
cmake ..
```
Installation de dependance : Cxx compileur,sql_priv.h

```
sudo apt-get install g++ 
sudo apt-get install build-essential
sudo apt-get install libncurses5-dev  
sudo apt-get install mysql-client libmysqlclient-dev
```
Configuration pour avoir Makefile

```
cmake ..
```
```  
sudo make
```
Installation 
```  
sudo make install
```
# APACHE

Telechargements des paquets sources  httpd-2.4.59.tar.bz2 dans des sites officielles comme APACHE .  
Commande :

```
tar -jxvf pour decompresser et desarchiver  httpd-2.4.59.tar.bz2 pour avoir httpd-2.4.59 .
```
	Commande : 	
```
 cd  httpd-2.4.59
 ls
 ./configure
```
Installation de dependance :Bison,APR,APR-util,pcre(2)
```
sudo apt-get install bison
sudo apt-get install libapr1 libapr1-dev
sudo apt-get install libaprutil1 libaprutil1-dev
sudo apt-get install libpcre3 libpcre3-dev
```
Configuration pour avoir Makefile
```
./configure
```
```
sudo make
```
Installation
```
sudo make install
cd
echo "export PATH='$PATH:/usr/local/apache2/bin'" >> .bachrc
```
<img src="https://github.com/mathieurazaka/Devoir-Linux-RAZAKANIRINA-Andrianina-Mathieu/blob/main/apache.png" alt="Capture_Apache" >
# PHP
	
Telechargements des paquets sources  php-8.1.28.tar.gz dans des sites officielles comme php.net .  
 
Commande :
```
tar -zxvf pour decompresser et desarchiver php-8.1.28.tar.gz pour avoir php-8.1.28 .
```
Commande : 
```
cd php-8.1.28 
ls 
./configure
```
Installation de dependance:libxml-cflags,libxml-libs,sqlite-cflags,sqlite-libs
```
sudo apt install pkg-config
export LIBXML_CFLAGS=$(pkg-config --cflags libxml-2.0)
export LIBXML_LIBS=$(pkg-config --libs libxml-2.0)
sudo apt install sqlite3 libsqlite3-dev pkg-config
export SQLITE_CFLAGS=$(pkg-config --cflags sqlite3)
export SQLITE_LIBS=$(pkg-config --libs sqlite3)
```
Configuration pour avoir Makefile
```
./configure
```
```
sudo make
```
Installation
```
sudo make install
```
