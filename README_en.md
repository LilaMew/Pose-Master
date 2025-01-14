# Pose Master Project Description

Machine translation, for reference only.

## What is this :no_mouth:
* This is a remote control project that uses a gesture sensor to capture hand motion signals to control objects.

## Appearance & How to Use :smiley_cat:
* It is a black rectangular device, with dimensions of 60mm * 50mm * 20mm and weighs approximately 50g.
* After connecting the remote controller to the object either wirelessly or through a wired connection, hold the remote with the top surface facing upwards. Control the object by moving your hand.
* For example, in the case of controlling a car: lean forward, and the car moves forward; lean backward, and the car moves backward; lean left, and the car turns left; lean right, and the car turns right. The greater the tilt angle, the faster the corresponding speed.
* During control, the button on the remote must be pressed. Once the button is released, the remote enters standby mode. In standby mode, the remote can be immediately woken up.

## Project Features :star:
1. The control method abandons traditional dual-stick precise control, opting instead for hand motion signals, providing an intuitive and easy-to-understand control interface that is simple to operate with one hand.
2. The signal transmission uses both wired and wireless options, ensuring stable object control in complex electromagnetic environments and at varying distances.
3. The size is much smaller than a traditional remote control, with an estimated total size not exceeding that of an ordinary IC card, easily fitting into a pocket for portability.
4. It uses a high-integration, multifunctional power management chip to precisely control current flow, charging modes, and current levels, ensuring stable power supply and overall system stability.
5. It includes a built-in lithium battery, allowing for some independent power capabilities.
6. The standby time is long, and it can be immediately woken up, with clear indicator lights.
7. The design is elegant, aesthetically pleasing, and resilient to extreme environmental conditions.

## System Architecture :four_leaf_clover:
![System Architecture](./system.png)
## Technical Solution
* Gesture Signal Algorithm: The MPU-9250 attitude sensor collects hand motion signals, which are filtered using a Kalman filter algorithm. The signal is then recognized by a posture recognition algorithm to output corresponding control signals.
* Signal Transmission: Both wired and wireless transmission are used to transmit control signals. The wired transmission uses the RS485 protocol, and the wireless transmission uses the 2.4GHz Wi-Fi protocol.
* Antenna Design: It uses both built-in and detachable external antennas to ensure signal transmission stability in different environments.

## Required Knowledge and Skills :books:
* Familiarity with embedded system development and C programming.
* Knowledge of the nRF52840 chip and its development environment.
* Familiarity with the MPU-9250 gesture sensor and its applications.
* Knowledge of various communication protocols such as UART, SPI, I2C, RS485, etc., and an understanding of Wi-Fi protocols.
* Knowledge of power management, including lithium battery charging and power management circuits.
* Familiarity with debuggers, programmers, and their applications.
* Understanding of how to handle interference, such as electromagnetic interference and temperature changes.
* Basic knowledge of the Kalman filter algorithm and its applications.
* Understanding of posture recognition algorithms and their applications.
* Knowledge of design thinking and basic principles and techniques of appearance design.
* Familiarity with PCB design and PCB fabrication.

## Application Scenarios :bullettrain_front:
* Drone control
* Autonomous vehicle control
* Robotic arm control

## Risk Assessment :zap:
* Hardware Design Risk: Hardware design needs to account for environmental factors such as electromagnetic interference and temperature changes, ensuring robustness. The nRF52840 chip has limited resources, so efficient utilization of these resources is required for system performance and stability. If the chip's performance is inadequate, consider switching to a more powerful chip.
* Software Development Risk: Software development must account for potential errors and exceptions, ensuring stability and reliability. The learning curve and development time should also be considered to control the project timeline.
* Supply Risk: The supply of hardware and software components may be impacted by factors such as changes in production schedules or delays in delivery, requiring stable and reliable supply management.
* Scheduling Risk: Project scheduling must consider factors like technical challenges, time constraints, and collaboration methods, ensuring proper control of the project timeline.

## Project Timeline :calendar:

| Team Member | Task                                                  | Date                             |
|-------------|-------------------------------------------------------|----------------------------------|
| LilaMew| 3D model design, overall circuit design, main code writing; overall project planning | Model design completed; others until final acceptance date |
| YiHuan| Design of wired and wireless communication, antenna design; communication-related code writing | Communication design until 2025/2/5; others as above |
| chu7-1| Design of power reset, programming buttons, circuit indicators, operation method design, usability study | Peripheral circuit design until 2025/1/20; others as above |

## Expected Project Outcomes :apple:
* Complete the design and development of the controller, excluding communication, and implement hand motion signal capture and processing.
* Achieve both wired and wireless signal transmission, ensuring stable control in different environments.
* Implement standby wake-up and indicator light functions.
* Develop a comprehensive set of operation methods.
* Deliver an elegant and aesthetically pleasing design to meet user appearance preferences.
* Ensure tolerance to extreme environmental conditions.