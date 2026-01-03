# PID Motor Control Project

Closed-loop DC motor speed control using a PID controller implemented on an embedded microcontroller.

## Overview
This project implements a real-time PID controller to regulate DC motor speed using encoder feedback.  
The controller was tuned and validated on physical hardware, with step response and steady-state performance measured experimentally.

## System Architecture
- DC motor with incremental encoder
- Embedded microcontroller (timer-based control loop)
- PWM motor driver
- UART for telemetry and tuning

(Control loop runs at fixed sampling rate using hardware timers.)

## Control Strategy
- Proportional–Integral–Derivative (PID) speed control
- Discrete-time implementation
- Anti-windup via integral clamping
- Tuned using step-response testing

## Results
- Stable closed-loop response
- Reduced steady-state error
- Improved rise time and overshoot control

See plots and test results in the `docs/` folder.

## Tools & Technologies
- Embedded C / C++
- Hardware timers & PWM
- Serial telemetry
- Control theory (PID)

## Future Improvements
- Feedforward control
- Auto-tuning
- Position control mode
