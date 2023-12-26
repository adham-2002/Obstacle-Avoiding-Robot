# Arduino Robot Car Project

This GitHub repository contains the code for an Arduino-based robot car project. The robot is equipped with ultrasonic sensors to detect obstacles and make decisions for navigation.
<img width="328" alt="Screenshot 2023-12-26 151025" src="https://github.com/adham20022023/Obstacle-Avoiding-Robot/assets/90427660/a337fc90-c08b-44d2-9dc0-4d4494774910">

## Hardware Components
- **Ultrasonic Sensors:**
  - Left Sensor: Echo1 (Pin 2), Trig1 (Pin 4)
  - Central Sensor: Echo2 (Pin 9), Trig2 (Pin 11)
  - Right Sensor: Echo3 (Pin 3), Trig3 (Pin 5)

- **Motor Control:**
  - Motor Pins: in1 (Pin 13), in2 (Pin 12), in3 (Pin 10), in4 (Pin 8)
  - Motor Speed Control: ENA (Pin 7), ENB (Pin 6)

- **Motor Speeds:**
  - Left Motor Speed: 135
  - Right Motor Speed: 215

- **Angular Velocities:**
  - Velocity: 0.04 cm/sec
  - Right Angular Velocity: 0.05 degree/sec
  - Left Angular Velocity: 0.05 degree/sec

- **Distances and Thresholds:**
  - Minimum Distance: 18 cm
  - Rotation Degree: 30 degrees

## Setup
1. Connect the ultrasonic sensors and motor control pins to the specified Arduino pins.
2. Adjust motor speeds and angular velocities as needed.

## Functions
- `move_F()`: Move the car forward.
- `move_B()`: Move the car backward.
- `move_R()`: Rotate the car to the right.
- `move_L()`: Rotate the car to the left.
- `STOP()`: Stop the car.
- `rotate_degree(float degree, char rotation_direction)`: Rotate the car by a specified degree and direction.
- `left_distance_read()`, `forward_distance_read()`, `right_distance_read()`: Read distances from the corresponding sensors.
- `sensor_testing()`: Continuous testing of sensor readings.

## Usage
1. Upload the code to your Arduino board.
2. Connect the robot to a power source.
3. Observe the robot's behavior in response to obstacles.

Feel free to modify the code according to your specific requirements and experiment with different parameters for optimal performance. If you encounter any issues or have suggestions for improvement, please feel free to open an issue or contribute to the project. Happy coding!
