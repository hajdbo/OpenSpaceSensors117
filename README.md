# OpenSpaceSensors 117

## What is it ?

OSS117 is a connected object made to control some environmental values for best performances at work.

## How it works ?

OSS117 is based on Intel Edison SoC with Grove sensors :

* Temperature
* Sound
* Dust
* Light
* Air quality

## See all steps on instructables.com

http://www.instructables.com/id/OPENSPACESENSORS-117-aka-OSS117/

## Why ?

This project was born in the Intel IoT Roadshow in Paris (12 & 13 September 2015). #IntelMaker

## How can i install it ?

Update your Edison :

    opkg update
    opkg upgrade
    
Edit /etc/opkg/base-feeds.conf :

    vi /etc/opkg/base-feeds.conf

and paste :

    src/gz all  http://repo.opkg.net/edison/repo/all
    src/gz edison  http://repo.opkg.net/edison/repo/edison
    src/gz core2-32 http://repo.opkg.net/edison/repo/core2-32
    
Re-update and install python-pip :
 
    opkg update
    opkg install python-pip

Install Flask :

    pip install flask
    
The Webserver is installed !

After that, launch the main.py :
    
    python main.py
    
(Optional) Launch the webserver if you want the Web Interface :

    python webserver.py

## Contributors

- Boris Hajduk
- Florent Kosmala
- François Dupayrat
- Hanlin Xu
