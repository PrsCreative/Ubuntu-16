# Ubuntu-16

## Downgrand PHP 7 to 5.6
  $ sudo apt-get purge `dpkg -l | grep php| awk '{print $2}' |tr "\n" " "`
  
  $ sudo add-apt-repository ppa:ondrej/php
  
  $ sudo apt-get update
  
  $ sudo apt-get install php5.6

## Install PHP Module Simple
  $ sudo apt-get install php5.6-mbstring php5.6-mcrypt php5.6-mysql php5.6-xml
  
  
  ## Install PHP 5.5 On Ubuntu 16
    Ubuntu 16 not create directory php5 in /var/etc/    เราต้องเป็น Create เอง

  $ sudo apt-get purge `dpkg -l | grep php| awk '{print $2}' |tr "\n" " "`
  
  $ sudo add-apt-repository ppa:ondrej/php5
  
  $ sudo apt-get update
  
  $ sudo apt-get install php5.5

## Install Extension form PHP 5.5
  $ sudo apt-get install php5.5-mbstring php5.5-mcrypt php5.5-mysql php5.5-xml php5.5-curl php5.5-gd
    
## Git command
  $ git add --all
  
  $ git commit -m " Message "
  
  $ git push origin master
  
  $ git status
  
  $ git fetch
  
  $ git clean --f
  
  $ git rm --cached test.dll
  
  $ git reset
  
## Create database UTF-8  
  $ CREATE DATABASE database_name DEFAULT CHARACTER SET utf8 DEFAULT COLLATE utf8_general_ci;
  
## Install PHP5.6 , 7.0
  $ sudo add-apt-repository ppa:ondrej/php

  $ sudo apt-get update

  $ sudo apt-get install -y php7.0 libapache2-mod-php7.0 php7.0 php7.0-common php7.0-gd php7.0-mysql php7.0-mcrypt php7.0-curl php7.0-intl php7.0-xsl php7.0-mbstring php7.0-zip php7.0-bcmath php7.0-iconv

  $ apt-get -y install php5.6 php5.6-mcrypt php5.6-mbstring php5.6-curl php5.6-cli php5.6-mysql php5.6-gd php5.6-intl php5.6-xsl php5.6-zip
  
## From php5.6 to php7.0 :
  
  ## Apache:
  
  $ sudo a2dismod php5.6 ; sudo a2enmod php7.0 ; sudo service apache2 restart

  ## CLI:
  
  $ update-alternatives --set php /usr/bin/php7.0
  
## From php7.0 to php5.6 :
  
  ## Apache:
  
  $ sudo a2dismod php7.0 ; sudo a2enmod php5.6 ; sudo service apache2 restart
  
  ## CLI:
  $ sudo update-alternatives --set php /usr/bin/php5.6

