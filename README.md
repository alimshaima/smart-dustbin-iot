# Smart Dustbin Using Arduino

## Description
An IoT-based smart dustbin that automatically opens its lid when someone approaches, using an Arduino Uno, HC-SR04 ultrasonic sensor, and a 9g servo motor. This touch-free waste disposal solution promotes hygiene and reduces physical contact with garbage bins.

## Features
- Automatic lid opening when person approaches within 50cm
- Touch-free operation for improved hygiene
- Low-cost and easy to build
- Adjustable distance threshold
- Servo motor for smooth lid movement

## Components Required
- Arduino Uno R3 - 1 piece
- HC-SR04 Ultrasonic Sensor - 1 piece
- 9g Micro Servo Motor - 1 piece
- Jumper Wires (M-M, M-F, F-F) - 10 to 15 pieces
- 9V Battery with DC Jack - 1 piece
- Small Dustbin with hinged lid - 1 piece

## Pin Connections
- Servo Signal → Arduino Pin 7
- Trig Pin (Ultrasonic) → Arduino Pin 5
- Echo Pin (Ultrasonic) → Arduino Pin 6
- LED Indicator → Arduino Pin 10
- Servo VCC → Arduino 5V
- Servo GND → Arduino GND
- Ultrasonic VCC → Arduino 5V
- Ultrasonic GND → Arduino GND

## Circuit Diagram
`circuit_diagram.jpeg` shows the circuit diagram of the smart dustbin setup.

## How It Works
- Ultrasonic sensor continuously sends out sound waves
- When an object comes within 50cm, the waves bounce back
- Arduino calculates the distance using time and speed of sound
- If distance is less than the threshold, servo motor rotates to open the lid
- After 3 to 5 seconds, servo returns to original position to close the lid

## Customization Options
- Change distance threshold: Modify `if (dist < 50)` in the code
- Change lid open delay: Modify `delay(3000)` in the code
- Change servo angle: Modify `servo.write(150)` value

## Installation and Upload Steps
- Clone this repository to your computer
- Open `smart_dustbin.ino` in Arduino IDE
- Select Board as Arduino Uno
- Select correct COM port
- Click the Upload button

## Expected Output
- When a person brings their hand within 10 to 15cm of the dustbin, the lid opens automatically within 1 second
- The lid remains open for 3 to 5 seconds
- The lid closes automatically without any manual contact

## Applications
- Hospitals to reduce infection spread
- Homes and kitchens
- Offices and public restrooms
- Schools and colleges
- Shopping malls

## Team Members
- Alima Shaima (4BP23CS004)
- Nishma (4BP23CS043)
- Rishma bibi Mariyam (4BP23CS045)
- Zaheera MA (4BP23CS063)

## Guide
Ms. Akshatha, Assistant Professor, Department of Computer Science and Engineering

## Institution
Bearys Institute of Technology, Mangaluru

## Author
Alima Shaima
