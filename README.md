# PHP-uploader-for-ShareX

This is a custom PHP uploader made for uploading files to your server with ShareX.

1. Create the upload folder in your webroot `mkdir i` and make sure that the folder used for uploading has at least 755 permissions. `sudo chmod 755 i`
1. Also change the owner and group of the upload folder to www-data (or equivalent). `sudo chown www-data:www-data i`

1. Place the upload.php to your webroot (eg. /var/www/example.com/upload.php) and the config.php to anywhere you like (just change the location in upload.php: `$config = include('config.php');`).

1. Open <b>ShareX</b>, click <b>Destinations</b>, click <b>Destination Settings</b>, scroll down until you find <b>Custom uploaders</b> and add a new uploader with following settings:

 ![ShareX settings](https://i.imgur.com/Ackyu7J.png)
