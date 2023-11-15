# Terminal som terminal

* I Windows ansluts terminalapplikationen till rätt COM-port och allt fungerar
* Mac/Linux har förfarande enligt UNIX, därav denna instruktion
* Installerade com-portar syns som ```tty``` (inbound teletype) eller ```cu``` (outbound call-up) under ```/dev```

## Hitta USB-port

* Öppna t.ex Iterm2

```ls /dev/cu*```
```ls /dev/ | grep cu.usbserial```

* Notera DEV-namnet på porten i listan
* Använd SCREEN kommandot i BASH

```screen /dev/cu.usbserial<portnamn> 115200```

## Lista SCREEN session

```screen -ls```

## Avsluta befintlig SCREEN session (för att kunna återansluta)

```screen -d 1643```

## iTerm2 specifikt

* Session - Status bar enabled - Composer
