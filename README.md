# Wordpress rename
A one-file developer-script for renaming URLs in your wordpress DB. I use this script quite often to move a wordpress installation from a test-subdomain to the real domain, or from localhost to the server.

## How to use
Prerequirements: All thinks are in place. You have setup your wp-config.php correctly, the DB is reachable ... and so on.

* [Download](https://raw.githubusercontent.com/vollyimnetz/wordpress_rename/master/rename.php) or checkout the script (`rename.php`) and place it in a public accessable directory. (Note: there is no authentication mechanism - delete the file once your ready.)
* create a `rename_config.php` file and add your settings.
* Open the script in your Browser and click the start-button.

## rename_config.php

	$GLOBALS['TM_RENAME_SETUP'] = array(
		'system' => __DIR__,            //Path to wp-load.php
		'old' => 'http://my-old-url.de',//Attention: without post-slash
		'new' => 'http://my-new-url.de',//Attention: without post-slash
	);
