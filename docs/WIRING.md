# Wiring

This is the wiring used by the current OpenShelf prototype.

The build uses a D1 Mini, a 6-pin SPI microSD module, and power filtering capacitors on a small perf board section.

---

## Pin Map

| Function | D1 Mini Pin |
|---|---|
| SD CS | D8 |
| SD SCK | D5 |
| SD MISO | D6 |
| SD MOSI | D7 |
| SD VCC | 3V3 |
| SD GND | GND |

The firmware currently defines the SD chip select pin as D8.

SPI uses the ESP8266’s default hardware SPI pins.

Default SPI mapping on the D1 Mini:

| SPI Function | D1 Mini Pin |
|---|---|
| SCK | D5 |
| MISO | D6 |
| MOSI | D7 |
| CS | D8 |

---

## microSD Module

The 6-pin SPI microSD module is wired directly to the D1 Mini SPI bus.

Module pinout:

| microSD Module | D1 Mini |
|---|---|
| CS | D8 |
| SCK / CLK | D5 |
| MISO / DO | D6 |
| MOSI / DI | D7 |
| VCC | 3V3 |
| GND | GND |

The current prototype uses a 32GB microSD card.

---

## Power

The D1 Mini is powered through its onboard Micro USB port.

The node can be powered using:

- Micro USB directly
- Micro USB male to USB-C female adapter

With the USB-C adapter installed, the adapter protrudes slightly from the enclosure.

Without the adapter, the Micro USB connection remains recessed inside the unit.

---

## Power Filtering

The current build includes:

- 100uF capacitor
- 104 ceramic capacitor

These are placed across the power rails for stability.

Placement:

3V3 → capacitor → GND

Both capacitors sit in parallel between 3V3 and GND.

This helps smooth power during Wi-Fi activity and SD card access.

---

## Perf Board Layout

The D1 Mini, SD module, and capacitors are mounted on a sawn section of perf board measuring approximately:

51.5 x 32 mm

The perf board acts as the internal mounting base and wiring platform.

---

## Notes

OpenShelf does not currently use external buttons, displays, sensors, or status LEDs.

All user interaction happens through the local Wi-Fi interface served by the D1 Mini.
