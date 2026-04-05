# Codes for my tournament-winning sumobots.

## Context
A sumobot (or robot-sumo) tournament is a competition in which two autonomous robots attempt to push each other out of a circular arena (like human sumo). I competed in the `mini` category, which restricts robots' dimensions to a 10x10 cm2 and its maximum weight to 500 g.

## Robots' Components
Both EspressoBot and MatchaBot contained:
- 1x Arduino Nano microcontroller, the "brain" of the bot
- 1x HC-SR04 Ultrasonic Sensor, which was used for "seeing" the opponent
- 2x QTR1A contrast sensor for edge detection
- 2x Core Dc Motor (6V 400 RPM) attached to a JS2114 Micro Silicone Wheel, both from JSumo
- 1x L298N Motor Driver for interfacing between the Arduino and the motors
- 1x 3d printed, cube-shaped carcass

## Approach and Outcomes

Both bots use a sliding-window moving average algorithm implemented with a circular buffer for O(1) IR sensor smoothing and noise rejection. MatchaBot iterated on EspressoBot's foundation, reducing IR noise readings from 8% to 3% and increasing main loop speed by 178% during opponent search. There was also CappuccinoBot, but we don't talk about it...


More info on each bot's README
