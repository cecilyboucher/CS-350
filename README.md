# Raspberry Pi Embedded Systems Projects

## Milestone 1 – PWM LED Fade Project

### Project Summary
This project demonstrates the use of **Pulse Width Modulation (PWM)** on a Raspberry Pi to create a smooth LED fade effect. Rather than simply turning the LED on or off, PWM controls brightness by rapidly switching the signal at varying duty cycles. The program continuously increases and decreases the LED brightness, creating a fade-in/fade-out effect until the user terminates the application.

### What I Did Well
- Implemented a clean shutdown process using `CTRL+C`.
- Properly stopped the PWM signal and cleaned up GPIO resources before exiting.
- Added clear comments throughout the code to improve readability and understanding.
- Structured the brightness adjustment logic to create a smooth visual transition.

### Areas for Improvement
- Replace hardcoded values (such as GPIO pin numbers and PWM frequency) with named constants for easier maintenance.
- Add runtime status messages to provide user feedback while the program is executing.
- Improve configurability by allowing users to adjust fade speed and brightness ranges.

### Tools and Resources Used
- **RPi.GPIO** library for GPIO and PWM control
- **Python `time` module** for timing and delays
- Raspberry Pi documentation
- PWM laboratory guide and course materials

### Transferable Skills
- Understanding and implementing PWM control
- GPIO programming and hardware interfacing
- Safe resource management and cleanup procedures
- Embedded systems programming fundamentals

### Maintainability and Adaptability
- Added comments to all major code sections.
- Kept the fade algorithm simple and easy to modify.
- Designed the code so brightness levels and fade speeds can be adjusted with minimal changes.
- Used a structured program flow that can be extended to other hardware control applications.

---

# Final Project – Smart Thermostat Prototype

### Project Summary
This project is a **smart thermostat prototype** built on a Raspberry Pi. The system monitors room temperature, displays information on an LCD screen, and uses colored LEDs to indicate operating status. A red LED represents heating mode, while a blue LED represents cooling mode. Users can interact with the thermostat through three buttons that allow mode selection and temperature adjustment. The system also sends a status update through the serial port every 30 seconds to simulate communication with a remote server.

### What I Did Well
- Implemented a state machine to manage thermostat modes (**Off**, **Heat**, and **Cool**) in a clean and organized manner.
- Created clear visual feedback using LED indicators:
  - Pulsing LEDs during active heating or cooling
  - Solid LEDs when the target temperature is reached
- Added proper shutdown handling to safely release hardware resources when the program exits.
- Organized functionality into separate classes for improved readability and maintainability.

### Areas for Improvement
- The temperature sensor currently uses a mock value; adding realistic fluctuations would improve testing.
- Implement temperature setpoint limits to prevent unrealistic user inputs.
- Replace hardcoded GPIO pins and configuration values with named constants.
- Expand error handling for sensor and communication failures.

### Tools and Resources Used
- **statemachine** library for mode management and transitions
- **gpiozero** library for GPIO devices
- **Python threading** module for background display updates
- **Python serial** library for UART communication
- Raspberry Pi hardware documentation and project guides

### Transferable Skills
- State machine design and implementation
- Multithreading and concurrent programming
- Event-driven programming with button inputs
- UART/serial communication
- Object-oriented software design
- Embedded systems architecture

### Maintainability and Adaptability
- Added comments to all classes and methods.
- Separated thermostat, display, and sensor functionality into independent classes.
- Designed the application with modular components that can be updated independently.
- Made it easy to switch from a mock temperature sensor to a physical sensor by changing only a few lines of code.
- Structured the code to support future hardware upgrades and feature additions.
