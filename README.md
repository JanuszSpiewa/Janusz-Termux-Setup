## Update termux repo and install apps:

apt update -y && apt full-upgrade -y && apt install python vim fish mc tor polipo proxychains-ng git perl go && curl -L https://raw.githubusercontent.com/OzakIOne/termux-youtube-dl/v1.0.1/install.sh | bash

##You must click allow premission to create storage/ folder

## Install speedtest-cli in termux:

git clone https://github.com/thelearn-tech/speedtest-cli

cd speedtest-cli

sh termux-install.sh

## Replace polipo  orginal config to secure config generate in Tor Developers:


cd /data/data/com.termux/files/usr/etc/polipo
mv config config.old 

cp /data/data/com.termux/files/home/Janusz-Termux-Setup/polipo.conf /data/data/com.termux/files/usr/etc/polipo 
	
	
## Change default shell:

Type : chsh

Termux ask You:

Changing the login shell
Enter the new value, or press ENTER for the default
        Login Shell [bash]:

Type fish and enter

Restart termux app 

## Replace motd file:
  rm /data/data/com.termux/files/usr/etc/motd    
  
  cp /data/data/com.termux/files/home/Janusz-Termux-Setup/motd /data/data/com.termux/files/usr/etc

Done

![screenshot](https://github.com/JanuszSpiewa/Janusz-Termux-Setup/blob/main/screenshot.jpg)
