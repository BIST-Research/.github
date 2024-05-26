Welcome! This GitHub organization houses code and other materials related to research conducted through the Bio Inspired Sciences and Engineering lab (BIST) at Virginia Tech. 

# Repository Overview

## [Batlib](https://github.com/BIST-Research/BatLib)
Contains:
- Tools for controlling lab instruments like the oscilloscopes and wavefunction generators through MATLAB
- Post processing tools for working with sonar data
Future work:
- Add more funcyionality to the lab instrument control code (include power supply implementation)
- Organize, refine and continue to develop the post processing tools that we currently use

## [EBatLib](https://github.com/BIST-Research/EBatLib)
This library houses the code used for developing some of the embedded applicaitons for our projects. Much more work needs to be done to this library in terms of organization and extensability. Although the SAMD51 micocontroller is somewhat outdated, it is still a very powerful chip with alot to offer. 
Future work:
- Continue extending library functionality, and maybe reframe the library to be more application specific to our lab. E.g., instead of having some generic ADC, DAC, DMAC, etc... (which still may be needed), instead, write implmentations for the sonar emission and reception systems, tendon actuation and force systems, etc...
- Integrate the motor control code into the embedded library
- Add preprocessing which can allow code to be run on any of the microcontroller boards we use (e.g., the sonar systems are written for the itsy bitsy m4 only). Although all the MCU boards we use (aside from Teensy 4.1) use the same microprocessor, the pinouts are different. 
- Move away from the arduino framework, and instead use Microchip's development suites. This should happen when the project moves towards more integrated hardware, e.g., the microcontroller is integrated onto our custom PCBs.

## [FieldBot](https://github.com/BIST-Research/fieldbot)
This repository houses the code which runs the sonar and gps systems on the field data collection rigs in the lab. As of May 2024, the main rover is now in Brunei, and this repository is maintained by the researchers who are there. 









