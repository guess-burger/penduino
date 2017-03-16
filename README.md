![Penduino Logo](https://github.com/guess-burger/penduino/raw/master/wiki/img/penduino.gif "Penduino Logo")

Penduino is a portmanteau of Pendulum and Arduino, and also a project I create at univeristy to produce a simple inverted pendulum using the Arduino micro-controller.
The project was originally hosted on Google Code where it stayed, somewhat abandoned but there seem to be a few forks floating around. 

The original idea was to make building an inverted pendulum a simple and cheap process.

![alt text](https://github.com/guess-burger/penduino/raw/master/wiki/img/robot.jpg "Penduino Logo")

The project was comprised of the hardware and software for small inverted pendulum robot as well as the control software for a balance telemetry and tuning app.

## Robot Hardware
The robot was comprised of Arduino duemilanove, 2 IR sensors, 2 full rotation servos, a pair of Xbee transciever modules.

![Hardware](https://github.com/guess-burger/penduino/raw/master/wiki/img/hardware_layout.png "Hardware")

## Robot Software
Penduino was written with re-use in mind and with the understanding that hardware could change. To this end, it contained a simple Arduino sketch that could be easily modified and some libraries, such as a tunable PID controller and pitch approximation. 



## Telemetry Software
![Telemetry screenshot](https://github.com/guess-burger/penduino/raw/master/wiki/img/telemetry.png "Telemetry screenshot")
The telemetry software provided a simple way to view the current angle of tilt along with tune the PID values the robot used.

It was originally written in Java and built with Maven2. 
It was comprised of 3 separate Maven projects; serial, core and gui which can be found under the Control directory.
Here is a diagram of how those components are linked
![Component diagram](https://github.com/guess-burger/penduino/raw/master/wiki/img/componet_class.png "Components")

