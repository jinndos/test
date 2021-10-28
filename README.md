# test

У меня получилось, вот тут по аналогии как можно поставить - там вообще как на любой дебиан на малинке поставить  https://github.com/Kanga-Who/home-assistant/blob/master/Supervised%20on%20Raspberry%20Pi%20with%20Debian.md 

Но если уже дошли до установки скрипта, то вместо него:

sudo apt --fix-broken install
sudo apt-get install udisks2 wget
cd /usr/local/src   

после чего инсталлируем OS Agent

sudo wget https://github.com/home-assistant/os-agent/releases/download/1.2.2/os-agent_1.2.2_linux_armv7.deb
dpkg -i os-agent_1.2.2_linux_armv7.deb

а потом сам HA - теперь он как инсталляция идет а не скрипт (внутри надо будет выбрать какая малинка у вас)

wget https://github.com/home-assistant/supervised-installer/releases/latest/download/homeassistant-supervised.deb
dpkg -i homeassistant-supervised.deb
