#PHPSass [![build status](https://travis-ci.org/richthegeek/phpsass.png)](https://travis-ci.org/richthegeek/phpsass)

## Use PHPSass with Apache
1. Copy/clone the file in the folder of your choice. (example: "sass")
2. Enable mod_actions. (command: "a2enmod actions")
3. Enable .htaccess files in /var/apache2/sites-enabled/*: Add line "AllowOverride All" in the VirtualHost
4. Reload Apache server. (command: "service apache2 restart")
4. Create an .htaccess in the folder where you can find the Sass/SCSS files. Put inside the two lines below:

`Action compile-sass /<NameOfFolder>/compile-apache.php` (`<NameOfFolder>` is the chosen folder in Step 1)

`AddHandler compile-sass .sass .scss`

_If you get an 404 ERROR, enable UseQueryString in the config.php file._

**Info: If you enabled UseQueryString in the config.php file, add a question mark after `compile-apache.php`**

## About
This is fork of PHamlP primarily for inclusiong as a Drupal pre-processor.
However, there is no Drupal-specific code and it will work for any PHP system.

This version of the compiler is NOT compatible with other forks of PHamlP, and
the name has been changed to reflect this.

## Other info
Origin: <http://code.google.com/p/phamlp/>

License: <http://www.opensource.org/licenses/bsd-license.php>

