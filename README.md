
```markdown
# Arduino Servo Motors Control Project

This project demonstrates how to control six servo motors using an Arduino UNO board. The aim is to create a walking motion for a robot using the Servo library to precisely control the servo motors.

## Components Needed
- Arduino UNO board
- Breadboard
- 6 Servo motors
- Jumper wires

## Circuit Connections
1. **Servo Motor Connections**:
    - Connect the signal wire of Servo motor 1 to pin 3 on the Arduino.
    - Connect the signal wire of Servo motor 2 to pin 5 on the Arduino.
    - Connect the signal wire of Servo motor 3 to pin 6 on the Arduino.
    - Connect the signal wire of Servo motor 4 to pin 9 on the Arduino.
    - Connect the signal wire of Servo motor 5 to pin 10 on the Arduino.
    - Connect the signal wire of Servo motor 6 to pin 11 on the Arduino.
    
2. **Power and Ground Connections**:
    - Connect the VCC (power) wire of each servo motor to the 5V line on the breadboard.
    - Connect the GND (ground) wire of each servo motor to the GND line on the breadboard.

## Code
Upload the following code to your Arduino to control the servo motors:

```cpp
#include <Servo.h>

Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;
Servo servo5;
Servo servo6;

void setup() {
  servo1.attach(3);  // Connect servo 1 to pin 3
  servo2.attach(5);  // Connect servo 2 to pin 5
  servo3.attach(6);  // Connect servo 3 to pin 6
  servo4.attach(9);  // Connect servo 4 to pin 9
  servo5.attach(10); // Connect servo 5 to pin 10
  servo6.attach(11); // Connect servo 6 to pin 11
}

void loop() {
  // Move the servos to create a walking motion for the robot

  // Move servo 1 and 4 to 90 degrees
  servo1.write(90);
  servo4.write(90);
  delay(500);  // Wait for half a second

  // Move servo 2 and 5 to 45 degrees
  servo2.write(45);
  servo5.write(45);
  delay(500);  // Wait for half a second

  // Move servo 3 and 6 to 135 degrees
  servo3.write(135);
  servo6.write(135);
  delay(500);  // Wait for half a second

  // Return servos to original positions
  servo1.write(0);
  servo2.write(0);
  servo3.write(0);
  servo4.write(0);
  servo5.write(0);
  servo6.write(0);

  delay(1000);  // Wait for 1 second
}
```

## Simulation on Tinkercad
To simulate this project on Tinkercad, follow these steps:
1. Create an account on [Tinkercad](https://www.tinkercad.com/) or log in if you already have one.
2. Click on "Circuits" from the side menu.
3. Click on "Create new Circuit".
4. Add the Arduino UNO and servo motors to the workspace.
5. Make the connections as described above and shown in the image below.
6. Copy and paste the provided code into the code editor in Tinkercad.
7. Click on "Start Simulation" to run the simulation and observe the servo motors' movement.

## Contributors
- **Mahmoud Al-Sharif** - Main Developer

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Image
Here is an image showing the connections used in the project:
![Project Connections](ddddddddddd.PNG)
```

This version includes a more detailed project description, step-by-step instructions for setting up the circuit and code, and clearer formatting to improve readability.
