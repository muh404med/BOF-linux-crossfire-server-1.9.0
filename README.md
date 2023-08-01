# BOF-linux-crossfire-server-1.9.0
three Python scripts showcasing different aspects of exploiting a buffer overflow vulnerability in "crossfire-server" version 1.9.0. The scripts demonstrate offset fuzzing, bad character identification, and a remote code execution exploit

#Install vunlerable service 

sudo wget www.offensive-security.com/crossfire.tar.gz
sudo tar -zxf crossfire.tar.gz
sudo cp -r crossfire /usr/games/

#Run 
sudo cd /usr/games/crossfire/bin/
sudo ./crossfire

