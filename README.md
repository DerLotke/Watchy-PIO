# Watchy for PlatformIO

![Watchy](https://watchy.sqfmi.com/img/watchy_render.png)

## What is this for?

This repository allows you to build different watchfaces for Watchy using PlatformIO with ease. This build system has been developed and tested under Linux, but it should also work for other operating systems that are supported by PlatformIO and your Python interpreter of choice.

## What is Watchy?

Watchy is a fully open source e-paper watch. Find out more at [**https://watchy.sqfmi.com**](https://watchy.sqfmi.com).

## Requirements

* PlatformIO
* Python3.11 or newer
* Watchy (using an ESP32-S3)

## Getting Started

1. Initialize the submodules by using `git submodule update --init`
2. Initialize the project with `pio project init`
3. Execute the configure script. A list of available watchfaces can be received via `./configure --list`, you can then use one of these names as an argument (e.g. `./configure 7_SEG`)
4. Build your watchface and upload it to your device (as convenience, you may use `make` and `make upload` for these tasks)
6. Have fun!
