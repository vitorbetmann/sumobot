# Codes for my tournament-winning sumobots.

## Context
A sumobot (or robot-sumo) torunament is a competition in which two autonomous robots attempt to push each other out of a circular arena (like human sumo).

## Robots' Components
Both EspressoBot and MatchaBot contained:
- 1x Arduino Nano microcontroller, the "brain" of the bot
- 1x HC-SR04 Ultrasonic Sensor, which was used for "seeing" the opponent
- 2x QTR1A contrast sensor for edge detection
- 2x Core Dc Motor (6V 400 RPM) attached to a JS2114 Micro Silicone Wheel, both from JSumo
- 1x L298N Motor Driver for interfacing between the Arduino and the motors
- 1x 3d printed, cube-shaped carcass

## Approach and Outcomes
More info on each bot's README
