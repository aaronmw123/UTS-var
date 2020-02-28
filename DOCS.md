sudo apt-get update

sudo apt install nginx mariadb-server mariadb-client php7.2 php7.2-fpm

sudo systemctl enable nginx

sudo service nginx start

sudo mysql_secure_installation

*unninstall mariadb*

sudo service mysql start

sudo mysql_secure_installation

mkdir "raka"

cd /etc/nginx/sites-available/

cp -t ~/raka default

*return to home folder*

mv -T default midtest

nano midtest

*changed the items*

sudo nginx -t

sudo ln -s /etc/nginx/sites-available/midtest /etc/nginx/sites-enabled/

sudo unlink /etc/nginx/sites-enabled/default

sudo nginx -t

sudo service nginx reload

cd /var/www/html/

nano info.php

*paste <?php phpinfo(); ?> to info.php*

*check browser localhost/info.php*

-------------------------------------------

wget http://lionwiki.0o.cz/download/3.2.11/lionwiki-3.2.11.zip

sudo apt install unzip

unzip lionwiki-3.2.11.zip

sudo cp -r lionwiki-3.2.11 /var/www/html/

cd lionwiki-3.2.11

sudo cp -r config.php /var/www/html/
sudo cp -r html /var/www/html/
sudo cp -r index.php /var/www/html/
sudo cp -r lang /var/www/html/
sudo cp -r plugins /var/www/html/
sudo cp -r templates /var/www/html/
sudo cp -r var /var/www/html/

nano index.php

*check browser for localhost/index.php*

*edit dan masukan text sesuai dengan template*
