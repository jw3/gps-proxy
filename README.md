bt gps
===

asset tracker type functionality over bluetooth



### bluetooth hardware

#### HC-05

Set up as master, first connection to bt slave

```
AT+ORGL
AT+ROLE=1
AT+RESET
AT+INIT
AT+PSWD=1234 #optional
AT+RMAAD
AT+PAIR=[csv-device-id],[connect-ttl]
AT+BIND=[csv-device-id]
AT+LINK=[csv-device-id]
```

After connected once, all that is needed is

```
AT+LINK=[csv-device-id]
```

Should look at putting the init into an exposed function call.

### gps hardware

#### dual 150a

password `1234`


### reference

- https://arduino.stackexchange.com/a/22403
