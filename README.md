# Telduino

## Summary
Telduino is an Arduino shield for land line telephones. Telduino has the ability to send and receive audio to and from land line telephones, as well as make them ring.

## Background
Over the last few years, I've been collecting interesting land line telephones here and there. Since land line service is nearly defunct as of this writing, I figured it would be neat to have a device that could pipe audio to and from a telephone and, more importantly, make them ring. This culminated in an Arduino shield that can be connected to a telephone.

## Details
The heart of this shield is the KS0835F SLIC (subscriber line interface circuit) module. This module provides all the required voltages, currents, and signals to the telephone. It also provides line level audio input and output. The module itself requires some signaling, which is provided by the Arduino.

The shield has two 3.5mm audio jacks for audio input and output, and a RJ11 jack for the telephone. The Arduino sketch controls ringing of the telephone by controlling the SLIC module.
