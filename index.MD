# Awesome utilities for developers and testers

## Command lines

### LINUX

**How to set a cronbtab execution**

Enter /etc/cdron.d folders. This folder can contains your custom script.

	cd /etc/cron.d

Create a file with your execution name

	nano name_of_your_execution_without_extension

Set some path in the script to permits to find binary position (not mandatory)

	SHELL=/bin/bash
	PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin

Set the cron. Remember to end the file with a empty line

	12 30    * * *   root    cd /home/ubuntu/cost-controlling-probes && python3 script.py

Remember 

* the format : min hour day month day of the week
* to give some minutes for crontab reload. avoid scheduling just a few minutes after the current "date".

**How to get crontab modifications**

	sudo tail -f /var/log/syslog

You should open a dedicated terminal in witch you run this command when you set a crontab execution to check if execution is registered.

**How to install another language (Useful if your python script use Locale)**

	sudo apt install language-pack-it-base language-pack-it

**How to get operative system date**

	date
	
**How to set ubuntu timezone**

	 sudo timedatectl set-timezone Europe/Rome

**How to get current timezone**
	
	timedatectl


### WINDOWS

## Software

## Image Generator
