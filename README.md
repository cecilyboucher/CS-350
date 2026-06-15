# Raspberry Pi Embedded Systems Projects

## Milestone 1 – PWM LED Fade

### Project Summary
Created a Raspberry Pi program that uses Pulse Width Modulation (PWM) to smoothly fade an LED in and out. The program continuously adjusts brightness until the user stops it.

### Strengths
- Implemented safe program shutdown using `CTRL+C`.
- Properly cleaned up GPIO resources.
- Added comments to improve readability.

### Areas for Improvement
- Replace hardcoded values with named constants.
- Add status messages for better user feedback.

### Tools & Resources
- RPi.GPIO
- Python `time` module
- Raspberry Pi documentation

### Skills Gained
- PWM control
- GPIO programming
- Embedded systems development
- Resource management

---

## Final Project – Smart Thermostat

### Project Summary
Built a smart thermostat prototype using a Raspberry Pi. The system displays temperature information on an LCD, uses LEDs to indicate heating and cooling states, accepts user input through buttons, and sends status updates through a serial connection.

### Strengths
- Used a state machine to manage operating modes.
- Provided visual feedback with LED indicators.
- Organized the project into separate classes for easier maintenance.
- Implemented safe shutdown procedures.

### Areas for Improvement
- Add realistic temperature simulation.
- Limit temperature setpoint ranges.
- Move hardware settings into configurable constants.

### Tools & Resources
- statemachine
- gpiozero
- Python threading
- Python serial

### Skills Gained
- State machine design
- Multithreading
- Serial communication
- Object-oriented programming
- Embedded systems architecture
