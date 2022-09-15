


## in main.js change following line to desired URL 


mainWindow.loadURL('http://localhost')


## run this commands to build electron rpm package 

sudo apt update
sudo apt install npm -y

sudo npm cache clean -f
sudo npm install -g n
sudo n stable

sudo npm install --global yarn

git clone https://github.com/ppp4ppp/electron-quick-start.git
cd electron-quick-start/

yarn add electron-builder --dev

sudo apt install ruby-full -y
sudo gem install public_suffix -v 4.0.7

sudo gem install fpm 

sudo apt-get install rpm -y
USE_SYSTEM_FPM=true yarn run electron-builder build --linux deb rpm --arm64 --armv7l
