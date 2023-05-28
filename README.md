##  _Installing Apache2_ 
```ssh
sudo apt update && apt upgrade 
sudo apt install apache2
```

## _Installing MariaDB_
```ssh
sudo apt update && apt upgrade 
sudo apt install apache2
sudo mysql_secure_installation
```
## _Installing PHP_

```ssh
sudo apt install php
sudo a2enmod php

```
## _Checking PHP configuration in Apache_
```ssh
echo "<?php phpinfo(); ?>" | sudo tee /var/www/html/index.html
sudo mv /var/www/html/index.html /var/www/html/index.php

```








## _Installing PHPMyAdmin_
```ssh
sudo apt install phpmyadmin
xdg-open http://localhost/phpmyadmin
```

