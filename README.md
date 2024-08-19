# Watchy for PlatformIO

![Watchy](https://watchy.sqfmi.com/img/watchy_render.png)

## What is this for?

This repository allows you to build different watchfaces for Watchy using PlatformIO with ease. This build system has been developed and tested under Linux, but it should also work for other operating systems that are supported by PlatformIO and your Python interpreter of choice.

## What is Watchy?

Watchy is a fully open source e-paper watch. Find out more at [**https://watchy.sqfmi.com**](https://watchy.sqfmi.com).

## Requirements

* PlatformIO
* Python 3.11 or newer
* Watchy v3 (using an ESP32-S3)

## Getting Started

1. Clone this project with `git clone`. A lot of functionality of the configure script abuses git commands to modify the submodules, so keep that in mind. ;)
2. Initialize the project with `pio project init` for your IDE.
3. Execute the configure script. A list of available watchfaces can be received via `./configure --list`. You can then use one of these names as an argument (e.g. `./configure 7_SEG`).
4. Build your watchface and upload it to your device (as convenience, you may use `make` and `make upload` for these tasks).
5. Have fun!

## Note on Settings Management

In order to avoid your `settings.h` being rewritten everytime you reconfigure the project, there is a template file present under `templates/settings.h.template` which you may edit.
This file will always be used instead of any `settings.h` file present in the watchface source.
