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
  $ sudo apt-get install php5.5-mbstring php5.5-mcrypt php5.5-mysql php5.5-xml

  $ apt-get install php5.5-gd

