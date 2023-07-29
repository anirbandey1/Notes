# Apache2

Install
```
sudo apt install apache2
systemctl status apache2
```


Firstly, we add the user pi (our user) to the www-data group, the default group for Apache2.

Secondly, we give ownership to all the files and folders in the /var/www/html directory to the www-data group.
```
sudo usermod -a -G www-data pi
sudo chown -R -f www-data:www-data /var/www/html
```
