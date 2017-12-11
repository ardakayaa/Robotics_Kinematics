# Pick and Place Project in ROS

This is my turn-in code as partial fulfillment of Udacity's Robotics Nanodegree. 
I wrote code to calculate the joint angles of six degree-of-freedom Kuka Kr210 serial manipulator given the position an orientation of its end effector in 3-D space. This code is used by the robot arm in a simulator to pick cylinders in a shelf 
and drop it in a bin. The simulation is implemented in a ROS environment with Gazebo and Rviz. 

# Changes
- **You can find images of results in the link below**
- - https://github.com/ardakayaa/Robotics_Kinematics/tree/master/img

# Notes

- **You can find the write up of the thought process in the link below**
- - https://github.com/ardakayaa/Robotics_Kinematics/blob/master/WriteUp.pdf


# Dependencies and Setup

- Install ROS on a computer with Ubuntu 16.04 Xenial
- - http://wiki.ros.org/kinetic/Installation/Ubuntu

- Clone Udacity's original repository
- - https://github.com/udacity/RoboND-Kinematics-Project

- Replace `IK_server.py` in `~/catkin_ws/src/RoboND-Kinematics-Project/kuka_arm/scripts` with the following script below:
- - https://github.com/ardakayaa/Robotics_Kinematics/blob/master/IK_server.py

- Follow the instructions as indicated in the README of the [original repository](https://github.com/udacity/RoboND-Kinematics-Project)


# Usage

- Make sure the demo flag is set to "false" in `inverse_kinematics.launch` file under `/RoboND-Kinematics-Project/kuka_arm/launch`

- Launch the project 
```
$ cd ~/catkin_ws/src/RoboND-Kinematics-Project/kuka_arm/scripts
$ ./safe_spawner.sh  
```

- On a separate terminal, run the inverse kinematics script
```
$ cd ~/catkin_ws/src/RoboND-Kinematics-Project/kuka_arm/scripts
$ rosrun kuka_arm IK_server.py
```

