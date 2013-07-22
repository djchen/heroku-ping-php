heroku-ping-php
===============

PHP script to ping your Heroku apps to keep them awake

You will need to configure a new app with 0 web dynos and 1 worker dyno

Edit the Procfile to change how often to ping your Heroku apps

Make sure you add the path to PHP extensions in the app config by running:

	heroku config:add LD_LIBRARY_PATH=/app/php/ext:/app/apache/lib

The index.php is just a dummy file so Heroku recognizes this as a PHP app
