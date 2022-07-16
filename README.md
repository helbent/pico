

Connect to serial console

1. Find port  

   `ls /dev/ttyACM*`

2. Connect to port

    `screen /dev/ttyACM0 115200`

   115200 is the speed in bits per second that the data is sent over the
   serial connection.

This will start the REPL. Note you may have code already running if you have code in  /media/helen/CIRCUITPY/code.py

Permissions problems:

Add yourself to the group:

```
ls -l /dev/ttyACM*
sudo adduser helen dialout
```
logout and log back in


Editing code:

Turn off swap files when using vim:

vim -n  /media/helen/CIRCUITPY/code.py


