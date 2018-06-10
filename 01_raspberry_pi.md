# Raspberry Pi

Onboard the vehicles outline in this project, a Raspberry Pi is used. You can use any revision of the Raspberry Pi, but the GPIO pin layout may be different (check if you use a different revision).

You will also need a micro SD card (pick up whatever is cheapest, any size will do).

- [Raspberry Pi 3 Model B ($39.00)](https://www.amazon.com/Raspberry-Pi-RASPBERRYPI3-MODB-1GB-Model-Motherboard/dp/B01CD5VC92/ref=sr_1_3?s=pc&ie=UTF8&qid=1528672676&sr=1-3&keywords=raspberry+pi+3)
- [16GB Micro SD card ($6.95)](https://www.amazon.com/SanDisk-Mobile-MicroSDHC-SDSDQM-B35A-Adapter/dp/B004ZIENBA/ref=sr_1_7?s=pc&ie=UTF8&qid=1528674430&sr=1-7&keywords=micro+SD+card)

## Setup

1. [Install Raspian OS onto your Raspberry Pi's SD card](https://www.raspberrypi.org/downloads/raspbian/) (choose "Lite" version, or Desktop if you prefer).
2. Follow [this guide](https://howchoo.com/g/ndy1zte2yjn/how-to-set-up-wifi-on-your-raspberry-pi-without-ethernet) ([archive.org](http://web.archive.org/web/20180610234348/https://howchoo.com/g/ndy1zte2yjn/how-to-set-up-wifi-on-your-raspberry-pi-without-ethernet)) to set up WiFi via the SD card.
3. Follow [this guide](https://howchoo.com/g/ote0ywmzywj/how-to-enable-ssh-on-raspbian-without-a-screen) ([archive.org](http://web.archive.org/web/20180610234510/https://howchoo.com/g/ote0ywmzywj/how-to-enable-ssh-on-raspbian-without-a-screen)) to set up SSH via the SD card.

## GPIO expansion board

The Raspberry Pi 3 by default has 24 usable GPIO pins. This means you can e.g. turn on and off 24 unique circuits (e.g. an LED).

For this project, we use a lot of GPIO pins. More than the Raspberry Pi allows for on its own. We use this expansion board:

- [SainSmart Raspberry Pi Infinity Cascade RPI GPIO Expansion Board IO Extend Adapter Module](https://www.amazon.com/gp/product/B00YXHIZTY/ref=oh_aui_search_detailpage?ie=UTF8&psc=1)

With the use of this board, you can use up to 32 GPIO pins (it gives you 8 additional ones).

(Note: the Amazon reviews are poor because it lacks good instructions, but we provide those here)

## Pin Mapping Diagram

[This article by Microsoft](https://docs.microsoft.com/en-us/windows/iot-core/learn-about-hardware/pinmappings/pinmappingsrpi) ([archive.org](https://web.archive.org/web/20180610233025/https://docs.microsoft.com/en-us/windows/iot-core/learn-about-hardware/pinmappings/pinmappingsrpi)) has a great diagram for the GPIO pin layout on Raspberry Pi 2 & 3:

![rp2_pinout](https://docs.microsoft.com/en-us/windows/iot-core/media/pinmappingsrpi/rp2_pinout.png)

