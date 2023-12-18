This repo is used to practice created a robot description using URDF and Xacro. 
Original robot
![image](https://github.com/bus0v/barrista_robot/assets/51008991/460d073f-f2c1-4086-b980-399d7b224f52)

Gazebo representation
![image](https://github.com/bus0v/barrista_robot/assets/51008991/83b42127-c49b-4c8c-ac67-7b71fa1d6041)

Rviz Representation
![image](https://github.com/bus0v/barrista_robot/assets/51008991/899223ad-d5c6-47e9-9016-88b032e01d35)

The urdf folder contains the urdf model, without any macros and can be launch with the urdf launch file. The xacro folder contains the same robot descriptions, but it is split up into various macros.

In both cases the description includes a mesh model of a laser scanner, and gazebo plugins. 
The plugins include a laser sensor plugin and a differential drive plugin. 

The launch files automatically 
* start gazebo
* load the robot description
* spawn the robot
* start rviz
* load the rviz configuration


  As a result the robot can be driven around by publishing to the /cmd_vel topic and the odom and laser data can be received on the /scan and /odom topics.
