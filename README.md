# Self Driving Car Models

This repositoey inlcuded various of applied models used in nowadays autonomous vehicles.

## kinematic bicycle model notebook
In this notebook, I implemented the kinematic bicycle model. The model accepts velocity and steering rate inputs and steps through the bicycle kinematic equations. We can provide a set of inputs to drive the bicycle in a certain trajectory.

The bicycle begins with zero initial conditions, has a maximum turning rate of 1.22 rad/s, a wheelbase length of 2m, and a length of 1.2m to its center of mass from the rear axle.

## longitudinal vehicle model notebook
In this notebook, I implemented the forward longitudinal vehicle model. The model accepts throttle inputs and steps through the longitudinal dynamic equations. We can give a set of inputs that drives over a small road slope to test your model.

The input to the model is a throttle percentage in range [0,1] which provides torque to the engine and subsequently accelerates the vehicle for forward motion.

## Controller2d
In this .py file, I implemented full logitudinal and lateral control of a simulated car in Carla software.

# State Estimation and Localization for Self-Driving Cars

## Extended Kalman Filter EKF
I implemented an Extended Kalman filter, which estimates the trajectory of a vehicle using odometry, range and bearing measurements.

## Error state EKF
Implementation of ES-EKF to predict the vehicle position depending on Data from IMU, Lidar and GNSS sensors.

# Visual Perception for Self-Driving Cars 

This notebook contains an inplementation to locate a car in a scene and estimate how far you are from it using a stereo camera model. This exercise gives a brief introduction to using Python to implement how to find the distance to collision with an obstacle.
