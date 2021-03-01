Using the same file from the previous chall, our objective now is to identify the ContainerID from the connected USB Device. Basically, a ContainerID is likely an identifier for a physical device when loaded intoan Operating system. After several research, we found a Volatility plugin named ​usbstor​​ that can be used to extract all information from an usb device. 

```
Commands Used: volatility --plugins=./volatility-plugins/ -f dump.raw --profile=Win7SP1x64 usbstor
```

Flag: vulncon{68b70eb8-f3fd-5099-907d-4e542601b2c7}
