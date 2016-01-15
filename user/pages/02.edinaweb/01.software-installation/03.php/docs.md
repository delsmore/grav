---
title: PHP
taxonomy:
    category:
        - docs
---

####Install PHP
	yum install php php-mysql

####Install PHP Modules
	yum install php-pdo.x86_64 php-gd.x6_64 php-pecl-memcache.x86_64 php-cli.x86_64 php-gd.x86_64 php-mbstring.x86_64 php-mysql.x86_64

####Restart Apache
	systemctl restart httpd.service

####Install Nano
	Yum install nano

####Create Info file
	nano /var/www/html/info.php
    
####Add following to info.php
	<?php phpinfo(); ?>
    

