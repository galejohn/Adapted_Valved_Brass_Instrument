# Adapted_Euphonium
​Robin Amend at https://amendmusiccenter.com​ made the first joystick-adapted euphonium in 1999, for a middle-school student in Mead, Washington. 

https://amendmusiccenter.com/assistive-technologies

Robin worked out a way to map joystick positions to valve positions that worked well for most beginner and intermediate brass music. He used an arcade joystick as the musician's user interface to control solenoids that pushed the 3 euphonium valves.



​​​​In 2018, Robin received a request for an adapted euphonium, from a music student in Illinois. He asked the students at the Spokane NEWTech Skill Center for help designing and building it.​
 ​

​​​​Our first prototype in 2018 used an Adafruit 32u4 Feather board:

https://learn.adafruit.com/adafruit-feather-32u4-bluefruit-le

with a PWM add-on board:

https://www.adafruit.com/product/2928​ 

to interpret the joystick input and to drive solenoids to push the euphonium valves. This worked, but the frequency of the Pulse Width Modulation (PWM) signal caused the solenoids to make an audible buzz when held active at a reduced power level.



We changed to an Adafruit nRF52 Feather board: 

https://learn.adafruit.com/bluefruit-nrf52-feather-learning-guide

which can do higher-frequency PWM without needing any add-on board.

To prevent burning up cheap solenoids, we activated them with full power, and then switched to lower 'Hold-in' power to hold the valves down.


In 2019, Robin had another request, for a trumpet. This time, we decided to use fast servos (typically used for RC model helicopter tail rotors and RC model car steering) to push the valves on the trumpet. These servos are lighter and use much less power than solenoids.

In 2025, we re-designed the euphonium setup to use servos instead of solenoids.

Please refer to the wiki for a description of the coding and design for the project.


