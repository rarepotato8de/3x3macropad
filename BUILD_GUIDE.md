# 3x3macropad - Build Guide


This guide provides a step-by-step explanation on how to solder/build the macropad.
Thanks to @mondrian for taking all of these pictures! He helped me so much with making this guide possible.

## Step 1: Soldering the HS Sockets and LED's
1.1 Get the PCB ready
![build_empty_pcb1](https://github.com/rarepotato8de/3x3macropad/assets/68034180/312e6a1e-a187-48a5-86ec-ed41a7ac7318)

1.2 Solder all of the Hotswap-Sockets you need (6 to 9, depending on your desired layout!) and optionally the LED's (The triangle/marked corner on the LED must align with the "triangle" corner on the PCB! It's diagonal from the "1" Text)
![build_hs_led_2](https://github.com/rarepotato8de/3x3macropad/assets/68034180/4593bf83-6fb2-4fca-b9a3-4ba3f969654c)


## Step 2: Soldering the Pro Micro
2.1 Split the Header Pins like shown in the picture, since a total of 4 Pins don't have through-holes in the PCB due to the layout
![build_promicro_pins_3](https://github.com/rarepotato8de/3x3macropad/assets/68034180/b22e9346-6962-411d-81f1-9f13c02ee0e7)

2.2 Insert the Header Pins like this in the PCB
![build_pins_pcb](https://github.com/rarepotato8de/3x3macropad/assets/68034180/8995bc9a-a2fb-4af4-ace2-50da6c54951c)

2.3 Place the Pro Micro on it (USB-Port facing towards the PCB!) and solder it's pins
![build_pins_promicro](https://github.com/rarepotato8de/3x3macropad/assets/68034180/9681533d-3b30-45ac-8efd-087e43d3854e)

2.4 Solder all the pins on the PCB
![build_pins_solder](https://github.com/rarepotato8de/3x3macropad/assets/68034180/9209efb0-76ee-4653-940c-fddef9097a3c)


# Step 3: Soldering the OLED and EC11 Encoder (both are optional)

3.1 Get some pliers and cut the already soldered pins as much as you can, but be careful. They still need to be soldered to the PCB!
![build_cut_top_pins](https://github.com/rarepotato8de/3x3macropad/assets/68034180/c300df85-f8ff-4f9d-8205-0795824eccf3)

3.2 Shorten these 5 Pins that are marked in the red boxes in the picture below. Otherwise they will interfere with the OLED
![cut_top_pins_both_done](https://github.com/rarepotato8de/3x3macropad/assets/68034180/df6113e0-6560-4097-8be2-02e9e7d4c7d0)

3.3 Get a knife or pliers and remove the black Pin Header that is on the "bottom" of the OLED Screen Pins. You can "push" them down usually.
![build_remove_pin_header_oled](https://github.com/rarepotato8de/3x3macropad/assets/68034180/6d4036c6-23f3-4bf3-b75d-26b284a1399a)

3.4 After that it should look like that. Then also shorten the top solder joints on the OLED, but also be careful here: Don't damage the soldered connection. 
We just want to have a little more space "above" the OLED, so the Switch Plate later fits above it.
![build_shorten_oled_pins](https://github.com/rarepotato8de/3x3macropad/assets/68034180/22193c83-13b0-4722-a089-bc4f82d213cb)

> [!TIP]
> Before proceeding to do the next step, get yourself some tape and stick it on the bottom of the oled. It's meant to prevent possibly shorting the OLED with our PCB.

3.5 Place the OLED on the PCB like this and solder the pins from the bottom side. Make sure to hold the OLED relatively "even", so it looks good at the end
![build_oled_on_pcb_flat](https://github.com/rarepotato8de/3x3macropad/assets/68034180/15ed7c01-acca-4b96-81e1-4af837b67f31)

3.6 Now place your EC11 Encoder in the top right and solder all of it's 5 Pins: 2 at the top and 3 at the bottom
![build_oled_on_pcb_flat_2](https://github.com/rarepotato8de/3x3macropad/assets/68034180/b49cd2f3-e031-4e88-9757-21124af0f934)


# Soldering done!

We are now done with the difficult part: The soldering. This is what it should now look from the bottom.
![image](https://github.com/rarepotato8de/3x3macropad/assets/68034180/7785b3c5-3549-4f51-a5e7-a5cad97743db)

# Step 4: Assembling the Macropad

4.1 Screw the 4 Standoffs to the bottom plate
![image](https://github.com/rarepotato8de/3x3macropad/assets/68034180/5bd23acb-6c5d-4e92-91d0-183371803163)

4.2 Place the PCB on the 4 Standoffs and screw it tight
![image](https://github.com/rarepotato8de/3x3macropad/assets/68034180/3b092929-6f55-47d9-80f8-033a6042d723)

4.2 Insert your Switches into the Plate (Note: The Switch at matrix [0, 1] and [1, 1] are north facing unlike all others!) and place it on the PCB
![image](https://github.com/rarepotato8de/3x3macropad/assets/68034180/67cc89c9-a956-4626-81f3-7341d1986a82)

4.3 Put the EC11 Encoder Knob and you Keycaps on
![build_done_off](https://github.com/rarepotato8de/3x3macropad/assets/68034180/bc069448-4a5c-4f62-824b-d274b31f6283)


# Done
Congratulations! 🎉 👏🏻 
You've build your very own 3x3macropad.
![build_done_on](https://github.com/rarepotato8de/3x3macropad/assets/68034180/3c4cf7c0-0c84-4d35-8628-012759ef27a1)


# Step 5: Flashing the Firmware 
5.1 The very last step to get the macropad running is flashing a firmware to the Arduino Pro Micro. for that, visit my [QMK/VIAL Guide](QMK_GUIDE.md)
