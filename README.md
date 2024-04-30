# pithy
raspberry pi word processor  

Goal: a minimal word processor that is intuitve (menus are easy to navigate via the keyboard, no coding or terminal experience required to operate), reliable (will not crash mid-project, can be used on a plane, in a train or in full sun), and syncs to remote storage when connected to wifi. 


# initial setup
- image sd card and include ssh
- ssh into the device and connect bluetooth devices using `bluetoothctl`
  - see the following article for (the commands)[https://bluedot.readthedocs.io/en/latest/pairpipi.html#using-the-command-line]

# Setup R clone 
- See https://gist.github.com/sissbruecker/c9263e237f5972e25d9d84b71dd89292

# Setup Wordprocessing app
- likely going with a fork of https://github.com/zerowriter/zerowriter1/tree/main
- but maybe https://github.com/RyWhal/TypeWryter?tab=readme-ov-file
- or just using text edit already on the machine... 

### Components List

- Raspberry Pi Zero 2W
- logitech k480 bluetooth keyboard
- waveshare 7.2 inch e-ink display
-  
