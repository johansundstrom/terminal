# Terminal as a terminal

* I Windows ansluts terminalapplikationen till rätt COM-port och allty fungerar
* I Mac/Linux är det mer UNIX-likt, därav denna instruktion
* Installerade com-portar syns som ```tty``` (inbound teletype) eller ```cu``` (outbound call-up) under ```/dev```

## Hitta USB-port

* ```ls /dev/ | grep cu.usbserial```

https://dtucker.co.uk/blog/the-definitve-guide-to-setting-up-a-usb-serial-adapter-and-iterm2-on-osx/
