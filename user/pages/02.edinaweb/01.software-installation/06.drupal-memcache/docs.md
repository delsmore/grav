---
title: 'Drupal Memcache'
published: true
taxonomy:
    category:
        - docs
---

####Install and enable Drupal Memcache module

	drush dl memcache
    drush en memcache

#####Edit settings.php to make memcache the default cache class by adding:

	$conf['cache_backends'][] = 'sites/all/modules/memcache/memcache.inc';
	$conf['cache_default_class'] = 'MemCacheDrupal';
    
>>>The cache_backends path needs to be adjusted based on where you installed
    the module.

#####Make sure the following line also exists, to ensure that the special cache_form bin is assigned to non-volatile storage:
    
	$conf['cache_class_cache_form'] = 'DrupalDatabaseCache';

#####Optionally also add the following two lines to tell Drupal not to bootstrap the database when serving cached pages to anonymous visitors:

	$conf['page_cache_without_database'] = TRUE;
	$conf['page_cache_invoke_hooks'] = FALSE;
  
>>>>>If setting page_cache_without_database to TRUE, you also have to set
    page_cache_invoke_hooks to FALSE or you'll see an error like "Fatal error:
    Call to undefined function module_list()".
