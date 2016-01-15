---
title: Memcached
published: true
taxonomy:
    category:
        - docs
---

>>>Memcached is an in-memory key-value store for small chunks of arbitrary data (strings, objects) from results of database calls, API calls, or page rendering.

####Install memcached

	yum install memcached libmemcached-tools
	yum install php5-dev php-pear make
	yum install php-pecl-memcache
    
####Edit memcache.ini

	nano /etc/php.d/memcache.ini

####Make sure the following lines are present

	extension=memcache.so
	memcache.hash_strategy="consistent"

####Edit memcached

	nano /etc/sysconfig/memcached
    
####Configure as below

	PORT="11211"
	USER="memcached"
	MAXCONN="1024"
	CACHESIZE="1024"
	OPTIONS="-l 127.0.0.1"

####Start memcached

	service memcached start
