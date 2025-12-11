## Functional parts build notes (to get the Printer up and running)

Start with the [Stock Voron Trident manual](https://github.com/VoronDesign/Voron-Trident/blob/main/Manual/Assembly_Manual_Trident.pdf).

Be aware that the vT Manual uses a 250mm Version of the Trident, so some dimensions may seem wrong if you build a 300mm/350mm Version.



### P. 48 Trident manual:

Skip this step, we use physical endstops and no hall effect ones.



### P. 56-60 Trident manual:

If you are building a 300mm machine you will need to start you screws from the second screw hole in the rails leaving the end holes open to allow space for T-nuts at later steps. Small reminder: The carriages are designed to slide along the rail easily. This unfortunately also includes sliding off the rails. Dropping the carriage likely irreparably damages it. ALWAYS put the little black rubber Carriage stoppers back on the rail (into the holes without screws) until your printer ist up and runnning!



### P. 100-101 Trident manual:

Skip these steps, you wont use either the inductive probe or a Cable chain on XY.



### P. 111 Trident manual:

Again, if you are building a bigger printer than the 250mm version, start at the outer holes and screw the rail down every second hole. Small reminder (again): The carriages are designed to slide along the rail easily. This unfortunately also includes sliding off the rails. Dropping the carriage likely irreparably damages it. ALWAYS put the little black rubber Carriage stoppers back on the rail (into the holes without screws) until your printer ist up and runnning!



### P.114 Trident manual:

Install all 4 screws on the right XY Joint.



### P. 115 Trident manual:

Leave this step out, you dont use a cable chain on X and Y.



### P. 122-123 Trident manual:

You use a different X carriage / Probe. Fix the belts with some tape and proceed with the belt Routing. After you routed the belts, fix them on the other side with some tape as well.



### P. 131-133 Trident manual:

Skip these steps, you will do it later after tap is assembled.



### P. 133 Trident manual:

X Carriage: After finishing the AB-Belts Routing, switch to the [TAP Manual](https://github.com/VoronDesign/Voron-Tap/tree/main/Manual). Optotap is used as the sensor.

Be sure to take a look into the R8\_errata.md document, it Highlights some important changes from the Manual and install the X Endstop switch.



### P. 33 Tap Manual:

After you have installed Tap successfully and have the AB belts fixed in the tap carriage, switch to page 134 of the Trident Manual.



### P. 135-137 Trident manual:

Skip these steps since you don't use the stock X carriage but instead you use tap.



### P. 144-145 \& 159 Trident manual:

You don't use this endstop. Your endstop is Tap.



### P. 162/163 Trident manual:

Switch to the [Stealthburner manual](https://github.com/VoronDesign/Voron-Stealthburner/tree/main/Manual).



### P. 13 Stealthburner manual:

You use a Toolhead PCB, so install these two heat inserts.



### P. 14 Stealthburner manual:

Skip



### P. 30 Stealthburner manual:

Follow [this Video Guide](https://www.youtube.com/watch?v=ly22qmB3NxE&t=1s) on how to set the gear mesh on your CW2.

Follow [this video Guide](https://www.youtube.com/watch?v=L1gxBCiE0pk) on how to set the Anti-Squish as well.



### P. 31 Stealthburner manual:

Skip for now, we will install our Version of the Anchor later.



### P. 34 Stealthburner manual:

You dont need to fix the Cable Cover down with the m3x6 BHCS now, you will need to access this later.



### P. 36-43 Stealthburner manual:

All Hotends are mounted in a similar pattern and pretty self-explaining, your hotend mount and hotend will look different.



### P. 46-51 Stealthburner manual:

Be very careful with the cables, you can easily rip them off the LED PCB which leads to this LED and the following ones not working.



### P. 53 Stealthburner manual:

Be sure that your fan blows in the right Direction. Look at the arrows on the fan. Additionally, the Sticker on the fan is on the back pointing towards the Hotend. You want the fan to blow air into the hotend, not trying to pull the air out. This destroys your fan and your whole hotend mount because of heatcreep.



### P. 56 Stealthburner manual:

You dont need to screw the 5015 fan into the SB Face, you will install the SB0000 Fan PCB there later.



### P. 58 Stealthburner manual:

All parts of the Stealthburner are now pretty much finished. Now you will need to install the Can-Board on there and do some basic wiring. Switch to the [SB2209 RP2040 Manual](https://github.com/bigtreetech/EBB/tree/master/EBB%20SB2209%20CAN%20(RP2040)/Build%20Guide).



### P. 02 SB2209 manual:

Now you need to screw down the 5015 fan with the SB0000 PCB :)



### P. 03/04 SB2209 manual:

You need to select Vin (24V) for all fans. Be sure to wire Gnd to Gnd and 24V to 24V! Otherwise you will experience magic smoke later.



### P. 05 SB2209 manual:

Skip



### P. 06 SB2209 manual:

Be sure to wire Gnd to Gnd, Signal to Signal and 24V to 24V! Otherwise you will experience magic smoke later.



### P. 13 SB2209 manual:

You Need to set the switch to 1: on; 2: on; 3: off; 4: on



### P. 15 SB2209 manual:

Skip



### P. 16 SB2209 manual:

Be sure to use the endstop labeled "To CAN\_Endstop" which is the one with the short wires.



### P. 18 SB2209 manual:

Skip



### P. 19 SB2209 manual:

Skip, Stealthburner will be assembled later.



### P. 24 SB2209 manual:

You will need to Strip down the Isolation a bit so you have enough cable length to connect the cable to the PSU and to the Can port. Go back to the Tap Manual page 34 now, flashing the toolhead will be done later.

Use the tight cable sleeve around the cable.



### P. 36 Tap manual:

Stealthburner and Tap are now completed and installed. Switch back to p. 164 of the original Trident manual.



### P. 173 Trident manual:

Rotate the din rails 90° compared to the original layout.



### P. 181-183 Trident manual:

Skip; Raspberry Pi mounting and 5v PSU mounting is not needed. Instead, mount the CB1 / CM4 on the Manta.



### P. 191 Trident manual:

You use the 3in6 Power Distributor instead.



### P. 195 Trident manual:

another small reminder, you don't use a 5v PSU.



### P. 196 Trident manual:

small reminder, you dont use a Raspberry Pi.



### P.198-200 Trident manual:

Skip; TAP is your Z-Endstop, your X Endstop sits on Tap and your Y endstop will be mounted on the A Motor mount later.



### P. 202-205 Trident manual:

Skip these steps, instead configure your Manta like this:

[M8P\_v2 Jumper / Driver marking](https://github.com/FORMBOT/Voron-Trident/blob/main/Diagrams/M8P_config.pdf)

Place a Jumper on all yellow marked pins and place the TMC2209s with attached heatsink on all driver ports with a blue circle after installing the jumpers.



### P. 210/211/216 Trident manual:

Leave the cables to the 5v PSU out.



### P. 217 Trident manual:

Skip, you dont use a standart Raspberry.



### P. 218 Trident manual:

The Z-Endstop cables are not needed.



P. 218-219/221-231/233-237 Trident manual:
For a better Overview of the wiring, use the [wiring diagram](https://github.com/FORMBOT/Voron-Trident/blob/main/Diagrams/Wiring%20Diagram%20of%20Trident%20R1%20Pro.pdf).

Connect the B motor (left motor) to X Motor, connect the A motor (right motor) to Y Motor.

Connect the CAN-Cable to the right CAN-Port on the M8P and 24V / GND to the 24V PSU. If you think the cables are not Long enough, you haven't done [this step](https://github.com/FORMBOT/Voron-Trident/tree/main/Build%20Notes#p-24-sb2209-manual).



P. 232 Trident manual:
Route the Y Endstop cable and the A Motor cables down like the B Motor cable (but on the right side of the printer).



### P. 242-244/257 Trident manual:

Skip these steps and instead mount the klipperscreen.



### P. 258 Trident manual:

Don't close the electronics compartment yet, you will need to acces this while flashing the boards.



### P. 281 Trident manual:

Use the big cable sleeve around the exhaust fan cable (if you use the stock exhaust).



#### Don't power on the printer if you are not 100% sure you wired everything correct!

#### And have a look into [this](https://github.com/FORMBOT/Voron-Trident/blob/main/Diagrams/Instruction%20of%20Trident%20R1%20Pro.pdf).

