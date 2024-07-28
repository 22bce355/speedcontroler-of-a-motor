# Speed Control System for BLDC Motors in Simulink

## Project Overview

This project focuses on designing and simulating a speed control system for Brushless DC (BLDC) motors using MATLAB Simulink. The system uses a Permanent Magnet Synchronous Machine (PMSM) with a trapezoidal back-EMF and Hall sensors to achieve precise motor control.

## Components Used

- Switching Logic Circuit
- Add Block
- Permanent Magnet Synchronous Machine (PMSM) with trapezoidal back-EMF and Hall sensors
- Bus Selector
- Scopes for Output
- Constant Input
- Gain Block
- PWM Drive Circuit
- 3-Phase PWM Inverter
- PID Controller
- MOSFET
- Power GUI (Discrete)
- DC Voltage Supply

## Steps Followed

1. **Select Permanent Magnet Synchronous Machine (PMSM):**
   - Modify the back electromotive force (EMF) to a trapezoidal waveform.
   - Set the number of phases to 3.
   - Use a bus selector to monitor the output.

2. **Configure Bus Selector for PMSM Parameters:**
   - Access and monitor parameters like rotor speed, current, and voltage.

3. **Switching Block for Hall Sensor Signals:**
   - Process the three digital signals from the Hall sensors.
   - Generate three logic signals for the PWM drive circuit.

4. **PWM Drive Circuit:**
   - Convert logic signals into six device driving signals.
   - Control the three-phase inverter.

5. **Three-Phase Inverter:**
   - Convert DC power to three-phase AC power.

6. **PID Control:**
   - Use rotor speed as feedback.
   - Compare feedback with desired speed and calculate the error signal.
   - Use a PID controller to maintain the desired speed.

7. **Connect PID Output to PWM Drive Circuit:**
   - Adjust the six device driving signals in real-time.

## Circuit Diagram
![image](https://github.com/user-attachments/assets/41e3d42a-e595-42e0-a302-ffc993c09b29)


## Subsystems

### Switching Logic Circuit
![image](https://github.com/user-attachments/assets/6ae33c5c-3d21-4834-9c01-54f4d7c4199c)

### PWM Drive Circuit
![image](https://github.com/user-attachments/assets/ea1b5b53-abc5-4246-b849-bf0ddf36e15d)

## Results

When the rotor speed is set to 20 rad/s..
![image](https://github.com/user-attachments/assets/8816663f-dc31-44f7-8982-220c32713aca)
![image](https://github.com/user-attachments/assets/3718521e-4f0b-4c80-b017-78a0583a6409)


