# Adaptive Cruise Control (ACC) System - Simulink Model

This project is a dynamic and realistic Adaptive Cruise Control (ACC) system developed using MATLAB Simulink. It features a PID control algorithm to maintain a safe following distance and adjust the vehicle's speed automatically.

## Features

- Dynamic Following Distance: Automatically adjusts the following distance based on the vehicle's speed.
- PID Control: Calculates acceleration and braking commands using a PID algorithm.
- Output Signal Saturation: Implements physical limits for realistic acceleration and braking values.
- Dynamic Scenario Simulation: Capable of simulating sudden braking by the leader vehicle using a Step block.

## Tools Used

- MATLAB & Simulink
- PID Controller block
- Integrator (1/s) block
- Sum block
- Saturation block
- Step block (or Signal Builder)

---

## Visuals and Results

Here are the key visuals and the final simulation results demonstrating the system's performance and stability.

### Simulink Model

The main Simulink model shows the complete ACC system architecture.

![Simulink Model](https://github.com/BeratKutluer/Adaptive-Cruise-Control/blob/main/model.png)

### Performance Graphs

The following graphs show the dynamic behavior of the system over time.

![Leader Car Position](https://github.com/BeratKutluer/Adaptive-Cruise-Control/blob/main/position1.png)
*This graph shows the leader car's position over time, confirming its steady forward movement.*

![Follower Car Position](https://github.com/BeratKutluer/Adaptive-Cruise-Control/blob/main/position.png)
*This graph shows the follower car's position, illustrating how it adapts to track the leader.*

![Leader Car Velocity](https://github.com/BeratKutluer/Adaptive-Cruise-Control/blob/main/velocity1.png)
*This graph confirms the leader car's constant velocity, which the follower car must match.*

![Follower Car Velocity](https://github.com/BeratKutluer/Adaptive-Cruise-Control/blob/main/velocity.png)
*This graph shows the follower car's velocity as it smoothly accelerates to match the leader.*

![Distance (d) between Cars](https://github.com/BeratKutluer/Adaptive-Cruise-Control/blob/main/d.png)
*This graph confirms the key result: the distance between the two cars remains stable and within a safe range, proving the controller's effectiveness.*

---

## Final Simulation Results

The simulation runs a scenario where the leader car accelerates, and the follower car reacts to maintain a safe distance.

* **Final Distance (d):** The system successfully maintains a final distance of approximately 10 meters.
* **Final Velocities:** Both the follower and leader cars reach a stable velocity, with the follower successfully matching the leader's speed.
* **PID Settings:** The final PID controller settings used for the successful simulation are P=1.81, I=1.510, D=0.75.
