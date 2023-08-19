# generic-doorbell-sniffer-esphome

EspHome config to sniff the signal from this specific unbranded generic doorbell using a cc1101 & esp32: 

![fum-Kqe-Qr-UN](https://github.com/Lehoooo/generic-doorbell-sniffer-esphome/assets/52742690/2bd8ed12-c952-45c9-89f1-14fcef44bff9)

Used for integrating into Scrypted (HKSV fake doorbell)

# Usage

* Install this library into your EspHome host: https://github.com/dbuezas/esphome-cc1101

* Create a new device in EspHome. Use the config provided in config.yaml

* Flash onto esp

* Connect the esp to the cc1101 according to the config
  ```
        18, // SCK
        19, // MISO
        23, // MOSI
        5, // CSN
        12, // GDO0
  ```

* Change the binary_sensor mqtt-publish action according to your needs

* Profit?

