# Watchy for PlatformIO

![Watchy](https://watchy.sqfmi.com/img/watchy_render.png)

## What is Watchy?

Watchy is a fully open source e-paper watch. Find out more at [**https://watchy.sqfmi.com**](https://watchy.sqfmi.com).

## Setup for CLI users (Linux)

1. Make sure you have [PlatformIO](https://platformio.org/) installed
2. Initialize the Watchy repository by using `git submodule update --init`
2. Initialize the project with `pio project init`
3. Execute the configure script and use one of the names of the watchfaces from `lib/Watchy/examples/WatchFaces` as an argument to populate the src folder (e.g. `./configure 7_SEG`)
4. Build the project with `make`
5. Upload the firmware with `make upload`
6. Have fun!

## Version Notes

This configuration is made to support firmware version 1.14.1 for ESP32-S3 based hardware.
