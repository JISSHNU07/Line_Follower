# Line Follower Robot  

This project demonstrates how to build a Line Follower Robot using Arduino Nano, L298N Motor Driver, and a 5-Channel IR Sensor Array. The robot autonomously follows a line based on contrasting colors (e.g., a black line on a white surface).  

---

## Components  
### Hardware  
1. **Arduino Nano**  
   - The microcontroller processes sensor input and controls the motors.  
2. **L298N Motor Driver**  
   - Drives the two DC motors by controlling their speed and direction.  
3. **5-Channel IR Sensor Array (HW 871)**  
   - Detects the line's position on the surface.  
4. **BO Motors (2)**  
   - Provide motion to the robot's wheels.  
5. **7.4V Battery**  
   - Powers the entire circuit, including motors and sensors.  
6. **Wheels (2)**  
   - Attached to the BO motors to enable movement.  
7. **Chassis**  
   - A base to mount all the components.  
8. **Jumper Wires**  
   - Used to connect components.

### Software  
- **Arduino IDE**  
  - To write and upload the code to the Arduino Nano.

---

## Working  

1. **IR Sensor Array**  
   - The 5-channel IR sensor detects the surface color beneath it.  
   - Each sensor outputs HIGH (1) on detecting a white surface and LOW (0) for a black surface (or vice versa).  

2. **Microcontroller (Arduino Nano)**  
   - The Arduino Nano reads the sensor array data to determine the position of the line relative to the robot.  
   - Based on the line’s position, the Arduino calculates appropriate motor speed and direction using predefined logic.

3. **Motor Driver (L298N)**  
   - The Arduino sends control signals to the motor driver.  
   - The motor driver adjusts the speed and rotation of the motors to align the robot along the line.  

4. **Robot Movement**  
   - If the line is centered, both motors rotate at the same speed, and the robot moves forward.  
   - If the line deviates, one motor slows down while the other speeds up to steer the robot back onto the line.  

---

This system ensures that the robot continuously tracks and follows the designated line.  
