# mechatronics-project

This project was done in my final year of BEng Mechatronic for the module Mechatronics 424. The project entails using the Siemens PLC Simatic S7-1200 CPU 1214C DC/DC/DC (6ES7214-1AE30-0XB0) to interface with the various components of the project. The project requires to use the HMI software InTouch Wonderware to create a user-friendly operating system.

## Connections to PLC Tutorbox
Please refer to the "PLC IO Connections.pdf" for the map of the tutorbox and its legends.

### Faulhaber Connections
* We are using the HSC1(High Speed Counter 1) Module on the PLC and this is used to read the encoder from the Faulhaber motor. The HSC1 is mapped to I0.0 and I0.1. Thus connect Channel A to I0.0 and Channel B to I0.1 of the Faulhaber controller blackbox. 

* The DIR(Direction) and PWM(Pulse Width Modulation) ports of the Faulhaber blackbox connects to Q0.1 and Q0.0 respectively. The PLC is configured to use the Pulse Module 1 for the Faulhaber motor, and this is mapped to Q0.0.

* To allow the DIR to output a voltage connect the 24V OUT of the tutorbox to the common black port between Q0.0 and Q0.1.

### DC Motor Connections
* The given DC Motor does not have a encoder, and thus the blackbox controller for the DC motor does not have a channel A,B ports. 

* We connect the DIR port of the DC motor controller blackbox to Q0.3 and the PWM port to Q0.2. We are using the second Pulse Module of the PLC, which is mapped to Q0.2.

* As with the Faulhaber, we connect the 24V OUT of the tutorbox to the common black port between Q0.2 and Q0.3.

## Watch Table Variables
TBC

## Wonderware Intouch
TBC
