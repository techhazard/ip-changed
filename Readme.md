#IP Check
### keep up-to-date on IP changes
I use this to check for changes on my server which has a dynamic IP

This writes the current external ipv4 address in a text file (defaults to /var/log/IP.txt) and checks against that every hour.
If it changes it will put a line in the file describing when and what the change was and updates the current ip.
It also notifies you of this change via pushbullet. I use this to be able to change my DNS setting with my registrar.

## dependencies

* python 2
* pushbullet.py (see installation)
* dig

## Installation

Install pushbullet.py:
* via pip: `pip install pushbullet.py`
* from source: see https://pypi.python.org/pypi/pushbullet.py/0.8.1

1. Put your Pushbullet API key in a file called `PUSHBULLET_API_KEY` next to the `IP-changed` script (see your account page on pushbullet.com )
2. run `./install`  
this will symlink IP-check to /etc/cron.hourly so it runs every hour  
and it will link IP-changed to /usr/local/bin  


## Removal
run `./remove`
this will remove the two symlinks

