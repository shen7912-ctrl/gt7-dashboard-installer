# GT7 Dashboard Custom Installer

Public Web Serial installer for the private **GT7 Dashboard Custom** firmware project.

Current test release: **v1.10.0**

Supported display targets:

- ESP32-2432S028 / ILI9341
- ST7789 build variant

The source firmware repository remains private. This repository contains only the installer, manifests, and compiled firmware images needed for browser installation.

## Browser support

Use Chrome or another Chromium-based browser with Web Serial support on desktop. Safari and Firefox do not currently support the required Web Serial API.

## First install

A first install writes the complete image from address `0x0`, including bootloader, A/B OTA partition table, boot metadata, and application firmware. Erasing the device is recommended for the first migration to this custom A/B layout.
