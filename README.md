# mercury
mercury dongle mw150uh linux driver install

Today I downloaded the linux driver for rt2870 from the official website of ralink(mediatek).
But in the zip file, I just found a xxx.dmg and I just did not know how to use it.

From the search results, it seems like some people had the same issue, and there is solution for it.
Here is the steps to do:

git clone https://github.com/porjo/mt7601.git 
cd mt7601/src
make
sudo make install
sudo mkdir -p /etc/Wireless/RT2870STA/
sudo cp RT2870STA.dat /etc/Wireless/RT2870STA/
sudo modprobe mt7601Usta

I just could not make the right result in the first command.

hzl@huazl:~$ git clone https://github.com/porjo/mt7601.git
Cloning into 'mt7601'...
Username for 'https://github.com': weixiufans
Password for 'https://weixiufans@github.com': 
remote: Repository not found.
fatal: repository 'https://github.com/porjo/mt7601.git/' not found


