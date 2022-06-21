# RPi Music Player
Simple Music player with web interface and GPIO input designed for Raspberry Pi. Web interface was implemented using Python Tornado, while GPIO handler was done using libgpiod library. Even though the project was created for RPi, the web interface script can be used with any Linux system.

## Prerequisites 

- RPi with GPIO buttons (without this kind of system, you still can use web player with any Unix/Linux system which supports the following software)
- Python Tornado package installed
- libgpiod library (if the project is used in the system with GPIO buttons) installed
- Change GPIO buttons IDs to yours in the gpio-player.py script
- mpd and mpc installed + set up mpd config and all related mpd files
- mpd should be started before the script

## Functionalities 

After starting the web-player.py script, you can manage playlist by uploading new music. You can also download the music from there and play/pause/change currently playing song. After playlist is set, you can also control music flow using GPIO buttons on the RPi.
