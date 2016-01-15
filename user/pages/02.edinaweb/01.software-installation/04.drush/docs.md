---
title: Drush
published: true
taxonomy:
    category:
        - docs
---

>>>Drush is a command line shell and Unix scripting interface for Drupal

####Download latest stable release 

	wget http://files.drush.org/drush.phar 


####Test your install

	php drush.phar core-status 

Make exectuable and rename to 'drush' instead of 'drush.phar'. Destination can be anywhere on $PATH. 

	chmod +x drush.phar 
	sudo mv drush.phar /usr/local/bin/drush

####Enrich the bash startup file with completion and aliases

	drush init
