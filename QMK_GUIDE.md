# 3x3macropad - QMK/VIAL Setup Guide

This guide provides a step-by-step explanation on how to set up QMK or VIAL, and how to modify, compile, and flash the firmware for your macropad.

## Table of Contents

1. [Preparation](#preparation)
2. [Downloading and Compiling QMK Firmware](#downloading-and-compiling-firmware)
3. [Resources](#resources)

## Preparation

Before you begin, make sure you have the following tools installed:
- [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases) - for flashing the firmwre
- [Python](https://www.python.org/downloads/) - for running QMK MSYS

## Downloading and Compiling Firmware

### Step 1: Setting up QMK MSYS
1. Install [QMK MSYS](https://msys.qmk.fm/), open it up and run this in the cmd:
   ```sh
   qmk setup
  After that, keep QMK MSYS open and follow the next steps.

### Step 2: Download QMK or VIAL Firmware

2. Clone the QMK firmware repository (within QMK MSYS!):
   ```sh
   git clone https://github.com/qmk/qmk_firmware.git
   cd qmk_firmware

**OR (preffered)**

2. Clone the VIAL firmware repository (within QMK MSYS!):
   ```sh
   git clone https://github.com/vial-kb/vial-qmk.git
   cd vial-qmk

3. optional: Modify the keymap under "keyboards/rarepotato8de/3x3macropad/keymaps/..." how you like (e.g. OLED): [HERE](https://docs.splitkb.com/hc/en-us/articles/360013811280-How-do-I-convert-an-image-for-use-on-an-OLED-display) is an awesome guide on how to get pictures on your OLED!

4. Compile the Firmware with the following command:
   ```sh
   qmk compile -kb rarepotato8de/3x3macropad -km default

   or for vial:

   qmk compile -kb rarepotato8de/3x3macropad -km vial
   
### Resources

- [QMK Documentation](https://docs.qmk.fm/)
- [VIAL Documentation](https://get.vial.today/docs/)
- [QMK Toolbox](https://github.com/qmk/qmk_toolbox)
- [Convert pictures for the OLED Screen](https://docs.splitkb.com/hc/en-us/articles/360013811280-How-do-I-convert-an-image-for-use-on-an-OLED-display)
