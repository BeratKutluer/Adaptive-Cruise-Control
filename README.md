# Adaptive Cruise Control (ACC) System - Simulink Model

This project is a dynamic and realistic Adaptive Cruise Control (ACC) system developed using MATLAB Simulink. It features a PID control algorithm to maintain a safe following distance and adjust the vehicle's speed automatically.

## Features

- **Dynamic Following Distance:** Automatically adjusts the following distance based on the vehicle's speed.
- **PID Control:** Calculates acceleration and braking commands using a PID algorithm.
- **Output Signal Saturation:** Implements physical limits for realistic acceleration and braking values.
- **Dynamic Scenario Simulation:** Capable of simulating sudden braking by the leader vehicle using a Step block.

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

![Simulink Model](https://github.com/YourUsername/YourRepoName/blob/main/path/to/your/image_124c8f.png)

### Final Simulation Results

The simulation runs a scenario where the leader car accelerates, and the follower car reacts to maintain a safe distance.

* **Final Distance (d):** The system successfully maintains a final distance of **10.0125 meters**.
* **Follower Car Velocity:** The follower car reaches a final velocity of **20.0249 m/s** to match the leader's speed.

### Performance Graphs

The following graphs show the dynamic behavior of the system over time.

![Position Graph](https://github.com/YourUsername/YourRepoName/blob/main/path/to/your/image_124ff4.png)

*The position graph shows both cars' positions, confirming the follower car successfully tracks the leader at a constant distance.*

![Velocity Graph](https://github.com/YourUsername/YourRepoName/blob/main/path/to/your/image_12506b.png)

*The velocity graph shows the follower car's speed reaching and stabilizing at the leader car's speed of 20 m/s.*
