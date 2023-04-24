---
title: "User Manual"
classes: wide

---

Click [here][1] to download a pdf of the user manual.

#### Turning the Extruder On
1. Precheck the Machine
*  Referencing the wiring logic diagram, **check that all the wires are appropriately attached.** Ensure that the grounding wires from the bus bars to the aluminum frame and housing are attached and secure.
*  Examine the motor train (motor, gear box, output shaft, coupler, flange, barrel) and **ensure that no wires or debris will impede rotation.**
*  Before continuing on to “Turning On Power”, **fasten all panels of the housing to the frame.**

2. **Turning On Power**
NOTE: Before you energize this system, know that the heating sections will immediately start to approach their setpoint. If you do not want the barrel to heat, your first step after attaching to wall power should be to adjust the set points of each PID down to 0 ℃. The PIDs only affect the control variable (temperature of the barrel) by manipulating the power to the heaters. If the set point is below ambient temperature, the heaters will not energize.
*  **Attach the external power cord to 110 VAC outlet.** 
    *  Upon attachment, the three PIDs’ screens should illuminate along with the VFD screen. The cooling fans may or may not turn on depending on the position of the potentiostat for each fan. In order to test if the fans are energized, adjust the knobs of each fan until the fan begins to turn.
      *  If any of the above devices do not energize, detach the power cord and begin troubleshooting.
*  **Adjust the setpoint of each of the PID controllers** to the desired temperature, and wait for the barrel to reach the desired temperature.
*  **Turn the feed section fan on.** The strength of this fan should be above half power as the feed section generally needs to be cool. 
* **Turn the compression and metering section fans** to a reasonable strength to keep the inside of the extruder cool.
*  **Fill the hopper with pellets or regrind** of your choosing.
*  **Select RUN on the VFD and adjust the knob to the desired frequency** in order to turn the screw. The VFD runs in frequency. Depending on the make and model of the motor in use, the rpm generally increases linearly with frequency. For example, for a 50 Hz motor with a max rpm of 1450, a 25 Hz setting results in 725 rpm. If you are using a 10:1 gearbox, this means the screw will turn at 72.5 rpm.
*  As you begin to extrude filament, **keep the hopper filled with pellets.**
*  **Collect your filament!**

3. **Turning Off Power**
*  **Reduce the VFD to 0 Hz then select STOP.**
*  **Adjust the setpoints of the PID controllers down to 0 ℃.**
*  **Adjust each of the fans down to no power.**
*  **Unattach the external power cord from wall power.**
NOTE: The barrel will NOT cool immediately. The extruder will remain hot even after turning off. Allow the extruder time to cool. If the extruder needs to be cooled quickly, keep the extruder attached to wall power, adjust the PID controllers to 0 ℃, and run each of the fans at full power until the desired barrel temperature is reached.
NOTE: VFDs function with very large capacitors that will continue to hold charge even after being disconnected from power. **Treat the VFD as if it is always powered.** 



[1]:{{ site.url }}/Extruder_User_Manual.pdf
