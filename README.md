# Arduino-Fan-Controller
A PCB board designed around an Arduino Nano to control temperature and lights in an enclosed electronics box.

..........................

CNC Arduino control board

Joe Asher
JAE design and manufacturing 8/31/2021

This board was created in order to control the climate inside an electronics box, as well as designed to act as a user interface to control lights inside the box as well.

The board will take inputs from two different one wire thermometers, one on the board, and the other a probe that can be placed at different locations around the box. These inputs are to be interpreted by the Arduino, and transistors will be controlled based on their resulting values. The trip temperatre that will activate the fan circuit will be 100°F or somwthing around that3, so when either one of the probes hits this temperature, the FAN pin will go high. If either one of the thermometers is disconnected or not functioning correctly, an error will come up on the display. This could very well change, and I might add a 4 pin fan to contorol via PWM. 

The board will also control the lights in side the electronics box. The user will be able to interface with the board using the single momentary switch and the small i2c display.

The board will be powered by an Antek power-supply that powers other electronics through the box. The PS provides +5v and +24v, so there is a circuit on the board to linearly convert +24v to +12v. The +5v will be used to power the electrionics on the board including the Arduino. The +12v will be used to power the Fan circuit for cooling. Finally the +24v is to be used for the LED light circuit.
This board has screw holes that will line up with 35mm din rail mounts. The following is a link to the mounts I designed it to work with.
https://www.amazon.com/gp/product/B083XY92LC/ref=ppx_yo_dt_b_search_asin_title? ie=UTF8&psc=1

..........................

