---
title: MariaDB
published: true
taxonomy:
    category:
        - docs
---

####Install MariaDB

	yum install mariadb-server mariadb

####Start

	systemctl start mariadb

####Configure

	mysql_secure_installation

####Start on boot

	systemctl enable mariadb.service

####Further tweaks
Edit `/etc/my.cnf`. 
Under the [mysqld] section add:

	max_allowed_packet = 64M
	wait_timeout = 6000
