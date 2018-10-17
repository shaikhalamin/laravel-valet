# laravel-valet
#https://cpriego.github.io/valet-linux/
#https://cpriego.github.io/valet-linux/requirements.html#1404

```php
//in order to work with valet composer must have present in your system

sudo apt-get install network-manager libnss3-tools jq xsel

sudo apt-get install php7.1-cli php7.1-curl php7.1-mcrypt php7.1-xml php7.1-zip php7.1-mbstring php7.1-mysql php7.1-pgsql


sudo add-apt-repository -y ppa:nginx/stable

sudo apt-get update

composer global require cpriego/valet-linux

//open bashrc file and put the following line for ubuntu 14.04
export PATH="$PATH:$HOME/.config/composer/vendor/bin"

//open bashrc file and put the following line for Ubuntu 17.04, 17.10 and 18.04:
export PATH="~/.config/composer/vendor/bin:$PATH"

//now reload bashrc file using the following command
source ~/.bashrc

//now run the valet command

valet install

//to test valet is working just ping foobar.test

//if you dont't want to .test domain then you can use .dev

//so in order to do that just run the following command

valet domain dev

#now create a directory in you home directory

mkdir Sites

cd Sites

#now run the following command to make this Sites directory to generate all folder under this directory as a domain

valet park

#now create any directory under sites and put index.php file there and open browser and type directoryname.dev and see the magic

```
