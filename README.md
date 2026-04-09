# PID Controller with Split Range Control

## Overview

This project demonstrates the implementation of an advanced PID control strategy using Split Range control in an industrial automation environment. The system was developed and tested using a PLC-based architecture with integration into a process simulation platform.

## Objective

The main objective of this project was to design and analyze a PID controller capable of controlling multiple final control elements using a single output signal. The system behavior was evaluated at different controller output levels (0%, 50%, 100%) to assess stability and transition performance.

## System Description

The control system uses a PID controller to regulate a process variable (e.g., pressure or level) by distributing the output signal across multiple actuators using Split Range logic.

* At low output levels → one actuator operates
* At higher output levels → another actuator takes control
* Smooth transition ensures stable process behavior

## Implementation

The system was implemented using:

* PLC controller (C300 architecture)
* PID function block
* FANOUT block for signal distribution
* AUTOMANUAL block for mode switching

According to the configuration shown in the project (see page 2–3), the PID parameters and signal ranges were carefully tuned to ensure stable operation without oscillations.

## Key Features

* Advanced PID control (P, I, D tuning)
* Split Range signal distribution
* Seamless transition between control elements
* Manual and automatic mode switching
* Real-time monitoring and parameter adjustment

## Simulation & Integration

The system was integrated with UniSim for real-time simulation and validation.

As shown on page 4, the simulation environment replicates industrial conditions, allowing:

* Testing under different loads
* Observation of controller response
* Validation before real-world deployment

## Results

The results demonstrated:

* Stable control performance without overshoot
* Smooth transition between actuators
* Reliable operation under varying conditions

The use of FANOUT and AUTOMANUAL blocks ensured coordinated control and operational flexibility. 

## Conclusion

This project provided practical experience in:

* Advanced PID control strategies
* Split Range control logic
* Industrial automation system design
* Simulation-based validation

The implementation reflects real-world industrial practices and highlights the importance of proper tuning and system integration. 
