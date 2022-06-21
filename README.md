# RPi Music Player
Simple Music player with web interface and GPIO input designed for Raspberry Pi. Web interface was implemented using Python Tornado, while GPIO handler was done using libgpiod library. Even though the project was created for RPi, the web interface script can be used with any Linux system.

## Prerequisites 

- RPi with GPIO buttons (without this kind of system, you still can use web player with any Unix/Linux system which supports the following software)
- Python Tornado and mpd packages installed
- libgpiod library (if the project is used in the system with GPIO buttons) installed
- Change GPIO buttons IDs to yours in the gpio-player.py script
- mpd and mpc installed + set up mpd config and all related mpd files

## How to start

1. Start mpd (if not started yet)
2. Execute the following commands:
  ```
  mpc clear
  mpc update
  mpc add /
  ```
3. Start web-player.py and gpio-player.py

## Functionalities 

After starting the web-player.py script, you can manage playlist by uploading new music. You can also download the music from there and play/pause/change currently playing song. After playlist is set, you can also control music flow using GPIO buttons on the RPi.
