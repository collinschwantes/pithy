# pithy
raspberry pi word processor  

Goal: a minimal word processor that is intuitve (menus are easy to navigate via the keyboard, no coding or terminal experience required to operate), reliable (will not crash mid-project, can be used on a plane, in a train or in full sun), and syncs to remote storage when connected to wifi. 


# initial setup
- image sd card and include ssh - https://www.raspberrypi.com/software/
- remember that some of the PIs can't connect to 5ghz networks
- ssh into the device and connect bluetooth devices using `bluetoothctl`
  - see the following article for (the commands)[https://bluedot.readthedocs.io/en/latest/pairpipi.html#using-the-command-line]
  - make sure the device and your machine are on the right networks

# Setup R clone 
- See https://gist.github.com/sissbruecker/c9263e237f5972e25d9d84b71dd89292
 - using rclone copy to move files from pithy to gdrive, using the `-cu` options to checksum and only update if pithy's files are newer
 - currently copying files every 5 mins 

# Connect e-ink to pi
- the connectors have little gates, open those up before trying to fit components together
- don't put the HAT on in the wrong orientation or it will get very hot very fast
- set display config to B and interface config to 0

# Setup Wordprocessing app
- likely going with a fork of https://github.com/zerowriter/zerowriter1/tree/main
- but maybe https://github.com/RyWhal/TypeWryter?tab=readme-ov-file
- or just using text edit already on the machine... 

### Components List

- Raspberry Pi Zero 2W
- optionally hdmi mini cable to make working with the pi a little easier
- logitech k480 bluetooth keyboard
- waveshare 7.2 inch e-ink display
  - there is a little lock on the bit that connects to the display. Lift up the black bar to attach.
  - https://www.waveshare.com/wiki/7.5inch_e-Paper_HAT_Manual#Working_With_Raspberry_Pi
  - https://www.waveshare.com/wiki/7.5inch_e-Paper_HAT_Manual#Python
