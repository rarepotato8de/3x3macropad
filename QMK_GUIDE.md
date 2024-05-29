# 3x3macropad - QMK/VIAL Setup Guide

This guide provides a step-by-step explanation on how to set up QMK or VIAL, and how to modify, compile, and flash the firmware for your macropad.


## Table of Contents

1. [Preparation](#preparation)
2. [Compiling the Firmware](#compiling-the-firmware)
3. [Flashing the Firmware](#flashing-the-firmware)
4. [Resources](#resources)


## Preparation

Before you begin, make sure you have the following tools installed:
- [QMK MSYS](https://msys.qmk.fm/) - for compiling the firmware
- [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases) - for flashing the firmwre 

## Compiling the Firmware

### Step 1: Setting up QMK MSYS
1. Install [QMK MSYS](https://msys.qmk.fm/), open it up and run this in the cmd:
   ```sh
   qmk setup
  After that, keep QMK MSYS open and follow the next steps.


### Step 2: Download QMK or VIAL Firmware

1. Clone the QMK firmware repository (within QMK MSYS!):
   ```sh
   git clone https://github.com/qmk/qmk_firmware.git
   cd qmk_firmware

**OR (preffered)**

1. Clone the VIAL firmware repository (within QMK MSYS!):
   ```sh
   git clone https://github.com/vial-kb/vial-qmk.git
   cd vial-qmk

2. optional: Modify the keymap under "keyboards/rarepotato8de/3x3macropad/keymaps/..." how you like (e.g. OLED): [HERE](https://docs.splitkb.com/hc/en-us/articles/360013811280-How-do-I-convert-an-image-for-use-on-an-OLED-display) is an awesome guide on how to get pictures on your OLED!

3. Compile the Firmware with the following command:
   ```sh
   qmk compile -kb rarepotato8de/3x3macropad -km default

   or for vial:

   qmk compile -kb rarepotato8de/3x3macropad -km vial


## Flashing the Firmware

### Step 1: Installing QMK Toolbox

1. Install [QMK Toolbox](https://github.com/qmk/qmk_toolbox) and open it up (preferably as administrator)

### Step 2: Configuration/ Settings

1. Select "atmega32u4" (Chip used on the ProMicro) in the top right
2. Select the "rarepotato8de_3x3macropad_*.bin" File that you compiled on the previous step. It's located in the main/root QMK or VIAL directory, depending on what you used previously
3. Tick the "Auto-Flash" Checkbox in the top right of QMK Toolbox for ease of use. Otherwise you manually need to press the "Flash" Button after the following step.

### Step 3: Flashing

1. Short the two pins at the top right on the PCB (where the Encoder is) with tweeters, scissors or whatever you have to connect both pins together. The Pro Micro should blink and QMK Toolbox will output some text in the console. At the end it should tell you that it's done ✅ 


## Done
Success! 🎉🤩 You can now use your macropad how you want. Have fun!


### Resources

- [QMK Documentation](https://docs.qmk.fm/)
- [VIAL Documentation](https://get.vial.today/docs/)
- [Convert pictures for the OLED Screen](https://docs.splitkb.com/hc/en-us/articles/360013811280-How-do-I-convert-an-image-for-use-on-an-OLED-display)
