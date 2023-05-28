# **` LAMP Alternative `**
` Tested in Debian GNU/Linux 11 (bullseye) x86_64 `



## **`1.Install Apache Server `**
```ssh
sudo apt update && apt upgrade 
sudo apt install apache2
```
 ## **`2.Install MariaDB `**
 `MariaDB is an open-source fork of MySQL.`
```ssh
sudo apt update && apt upgrade 
sudo apt install apache2
```
 ## **`4.Perform secure installation of MariaDB `**
`You can change the password of default user <root> to avoid future error in some cases.`
```ssh
sudo mysql_secure_installation
```
 ## **`5.Install PHP `**
```ssh
sudo apt install php
sudo a2enmod php
```
 ## **`6.Check PHP module in Apache `**
 `By executing the code below, php information page will open.`
```ssh
echo "<?php phpinfo(); ?>" | sudo tee /var/www/html/index.html
sudo mv /var/www/html/index.html /var/www/html/index.php
xdg-open http://localhost
```
 ## **`7.Install phpMyAdmin `**
 `phpMyAdmin provides GUI for MariaDB`
```ssh
sudo apt install phpmyadmin
xdg-open http://localhost/phpmyadmin
```


