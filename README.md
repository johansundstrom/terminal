# Terminal som terminal

* I Windows ansluts terminalapplikationen till rätt COM-port och allt fungerar
* Mac/Linux har förfarande enligt UNIX, därav denna instruktion
* Installerade com-portar syns som ```tty``` (inbound teletype) eller ```cu``` (outbound call-up) under ```/dev```

## Hitta USB-port

* Öppna t.ex Iterm2

```ls /dev/ | grep cu.usbserial```

* Notera riktiga namnet på porten i listan
* Använd SCREEN kommandot i BASH

```screen /dev/cu.usbserial<portnamn> 115200```
