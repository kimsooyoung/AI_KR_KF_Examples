# AI_KR_KF_Examples
AI Robotics Korea Sensor Fusion Study

# Robot localization Example for Odometry Sensor Fusion

![sf_study](https://user-images.githubusercontent.com/12381733/88390328-17e74180-cdf3-11ea-82f2-4080b9808aad.png)

# Setup

* Mac OS
* Windows
* Linux

> My Environment

- Ubuntu 18.04
- ROS Melodic

### Add noise to Kobuki's Odom

```
roslaunch turtlebot_localization turtlebot_bf_fusion.launch
```

### EKF Fusion

```
roslaunch turtlebot_localization turtlebot_af_fusion_ekf.launch
```

### UKF Fusion

```
roslaunch turtlebot_localization turtlebot_af_fusion_ukf.launch
```

### Fusion Comparision

Add those topic to `rqt_plot`

```
/odom/pose/pose/position/x
/odom/pose/pose/position/y
/noisy_odom/pose/pose/position/x
/noisy_odom/pose/pose/position/y
/odometry/filtered/pose/pose/position/x
/odometry/filtered/pose/pose/position/y
```

## Reference

* My Brain
* Robot Localization