# EKF-Slam
### EKF SLAM: Enhanced Kinematic-Based Robot Simulation with Adaptive Noise Models and PID Control

This repository contains a comprehensive simulation of robot navigation and landmark mapping using the Extended Kalman Filter (EKF) for Simultaneous Localization and Mapping (SLAM). The primary goal is to accurately estimate the robot's trajectory and surrounding landmarks within a simulated environment.

#### Features and Implementation Details:

* **Extended Kalman Filter (EKF) SLAM:**

  * Implements prediction and update steps to recursively estimate robot state and landmark positions.
  * Utilizes motion and measurement Jacobians for state prediction and covariance updates.

* **Kinematic Motion Model:**

  * Accurately simulates robot motion based on velocity commands, integrating kinematic equations.

* **Sensor Integration:**

  * Incorporates multiple sensor models including GPS and IMU.
  * GPS provides noisy positional updates, while IMU simulates noisy velocity measurements.

* **Adaptive Noise Models:**

  * Dynamically adjusts sensor noise levels based on robot velocities to enhance robustness and accuracy.

* **PID Controller for Angular Velocity:**

  * Employs a PID controller to calculate and adjust angular velocity, ensuring smooth and precise path tracking.
  * Features tunable parameters (Kp, Ki, Kd) to refine responsiveness and stability.

* **Error and Performance Analysis:**

  * Calculates Root Mean Square Error (RMSE) for both robot trajectory and landmark estimation.
  * Achieves trajectory RMSE of approximately **0.10 meters** and landmark RMSE of approximately **0.46 meters**.

#### Simulation Environment:

* Randomly generated landmarks within a defined environment size.
* End location guidance for the robot, driving autonomous navigation towards a goal.

#### Visualization:

* Provides visual plots comparing the true trajectory versus estimated paths and landmarks.
* Clearly demonstrates effectiveness and areas for improvement in EKF SLAM performance.

#### Future Enhancements:

* Integration of additional sensor modalities for enhanced accuracy.
* Sophisticated noise modeling approaches.
* Expansion to dynamic environments with mobile landmarks.

This project serves as a robust framework for further research in robotic navigation and mapping, inviting collaboration and further development.
