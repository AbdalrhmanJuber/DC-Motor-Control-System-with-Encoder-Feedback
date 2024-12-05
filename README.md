# DC-Motor-Control-System-with-Encoder-Feedback
This Arduino-based project demonstrates a DC motor control system using an L293D motor driver, a potentiometer, and an incremental encoder for feedback. The system is designed to adjust the motor's speed and direction dynamically based on the potentiometer input and display real-time feedback on an LCD screen.

Features:
Speed Control: The motor's speed is controlled by mapping the potentiometer's analog input to a PWM signal.
Direction Control: The motor's direction is determined by the polarity of the potentiometer input.
Forward (FWD)
Reverse (REV)
Stop (when input is neutral)
Encoder Feedback: An incremental encoder tracks the motor's position in real-time and updates the LCD and Serial Monitor.
LCD Display:
Displays motor speed and direction.
Shows encoder position.
Components Used:
Arduino Uno
L293D Motor Driver
DC Motor
Incremental Encoder
16x2 LCD Display
Potentiometer
Power Supply
How It Works:
Potentiometer Input:

Reads analog values from the potentiometer (0-1023) and maps them to motor speed (-255 to 255).
Positive values set the motor to forward rotation; negative values set it to reverse.
Zero value stops the motor.
Motor Control:

Direction: Controlled via IN1 and IN2 pins on the L293D driver.
Speed: Controlled using PWM on the ENA pin.
Encoder Feedback:

Tracks the motor shaft's rotation using interrupts.
Displays the encoder position on the Serial Monitor and the LCD.
LCD Display:

First Row: Motor speed.
Second Row: Direction and encoder position.
How to Run the Project:
Wire the components as per the circuit diagram.
Upload the code to the Arduino.
Adjust the potentiometer to control the motor speed and direction.
Monitor the motor's behavior and encoder feedback on the LCD or Serial Monitor.
Potential Applications:
Robotics and automation systems.
Motorized systems requiring precise speed and position control.
Educational projects for learning motor control and feedback systems.
