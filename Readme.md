# PicoSCSI

## A SD sard to Parallel SCSI hard drive emulator

### Board

The board design is lossely based on the [BlueSCSI V1](https://github.com/erichelgeson/BlueSCSI) and the [ZuluSCSI Pico](https://github.com/ZuluSCSI/ZuluSCSI-Pico-OSHW).
The [RP2350](https://www.raspberrypi.com/products/rp2350/) the MCU on the [Raspberry PI Pico 2](https://www.raspberrypi.com/products/raspberry-pi-pico-2/) is [5V tollerant](https://www.raspberrypi.com/news/rp2350-a4-rp2354-and-a-new-hacking-challenge/) meaning no level translation logic is nessasary.
Like BlueSCSI this outputs 3.3V to the bus, which is compliant with LV SCSI.

#### Documents relating to 5V tollerance
[Piers Finlayson's video](https://www.youtube.com/watch?v=Zy8IMe6fMI4&t=1768s) on the RP2350 variant of
[one-rom](https://github.com/piersfinlayson/one-rom/blob/main/sdrr-pcb/verified/rp2350-24-pin-rev-a/one-rom-24-pin-rp2350-rev-a-schematic.pdf) talks about caveats this may have.
The A4 silicon revision adds support for this https://www.raspberrypi.com/news/rp2350-a4-rp2354-and-a-new-hacking-challenge noted at the bottom.

### Firmware

Coming soon will be based on [ZuluSCSI firmware](https://github.com/ZuluSCSI/ZuluSCSI-firmware)

### TODO:

Add both SMD and THT versions
Add DB25 version
Fix Pi Pico not having combined THT and SMD footprint
