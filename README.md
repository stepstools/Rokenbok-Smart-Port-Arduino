# smart_port_arduino
An Arduino sketch that listens to commands from its serial interface to perform commands via the Rokenbok Smart Port protocol.

## Smart Port Pinout

![Smart Port Pinout](./mini-DIN-6.png)

| Smart Port | Arduino | Function |
|---|---|---|
| 1 | 13 | Serial Clock |
| 2 | 12 | MISO |
| 3 | 11 | MOSI |
| 4 | - | Frame End |
| 5 | 8 | Slave Ready |
| 6 | GND | Ground |
| - | 9 * | Chip Select (Virtual) |
| - | 10 * | Chip Select |

*\* Arduino pins 9 and 10 connect to each other instead for chip select simulation.

## Other Projects

### https://github.com/csev1755/rokenbok-webserver

A Python Flask executable that serves a Rokenbok multiplayer web interface with optional live video. Integrates with this Arduino implementation for Smart Port control.

### https://github.com/stepstools/Rokenbok-Smart-Port-WiFi

Custom ESP32 Smart Port interface with web control.
