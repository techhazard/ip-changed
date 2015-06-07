#IP Check
### keep up-to-date on IP changes
I use this to check for changes on my server which has a dynamic IP

## dependencies

* python 2
* pushbullet.py (see installation)
* dig

## Installation

Install pushbullet.py:
* via pip: `pip install pushbullet.py`
* from source: see https://pypi.python.org/pypi/pushbullet.py/0.8.1

Put your Pushbullet API key in the IP-changed script (see your account page on pushbullet.com )  
run `./install`  
this will symlink IP-check to /etc/cron.hourly so it runs every hour  
and it will link IP-changed to /usr/local/bin  



## Removal
run `./remove`
this will remove the two symlinks

