# Self_Driving_Car_Models

This repositoey inlcuded various of simple models used in autonomous vehicles.


## kinematic bicycle model notebook
In this notebook, I implemented the kinematic bicycle model. The model accepts velocity and steering rate inputs and steps through the bicycle kinematic equations. We can provide a set of inputs to drive the bicycle in a certain trajectory.

The bicycle kinematics are governed by the following set of equations:

  \begin{align*}
  <img src="https://render.githubusercontent.com/render/math?math=e^{i \pi} = -1">
  \dot{x}_c &= v \cos{(\theta + \beta)} \\
  \dot{y}_c &= v \sin{(\theta + \beta)} \\
  \dot{\theta} &= \frac{v \cos{\beta} \tan{\delta}}{L} \\
  \dot{\delta} &= \omega \\
  \beta &= \tan^{-1}(\frac{l_r \tan{\delta}}{L})
  \end{align*}


where the inputs are the bicycle speed $v$ and steering angle rate $\omega$. The input can also directly be the steering angle $\delta$ rather than its rate in the simplified case. The Python model will allow us both implementations.

The bicycle begins with zero initial conditions, has a maximum turning rate of 1.22 rad/s, a wheelbase length of 2m, and a length of 1.2m to its center of mass from the rear axle.
