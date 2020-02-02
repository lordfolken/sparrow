# Sparrow Box Installation

## OS Media

### Download ISO
Grab OpenSUSE Network boot image (15.1):

[leap 15.1](https://download.opensuse.org/distribution/leap/15.1/iso/openSUSE-Leap-15.1-NET-x86_64.iso)

### create usb bootstick
Dump image to usb stick (here sdc):

```bash
dd if=openSUSE-Leap-15.1-NET-x86_64.iso of=/dev/sdc bs=4096
```

## Configure PC for access to APU2 Serial terminal
Hook up serial terminal of APU2 Board note: 115200 baud rate!:

```bash
screen /dev/ttyUSB0 115200
```

## Boot USB stick on APU2
on the apu boot opensuse installer:

```bash
linux console=ttyS0,115200 textmode=1
```

## OS Installation
Setup Opensuse 
  * Timezone UTC
  * Server OS
  * disk parititoning currently btrfs default

## 
