# robot_auto_nav
Robot_auto_nav is a ROS package for implementing autonomous navigation in a Differential Drive Mobile Robot. The Mobile robot system is driven by two Nissei BLDC Motors, controlled through Arduino microcontroller. The entire package runs in [Robot Operating System (ROS)](https://www.ros.org/)and [ROS Navigation Stack](http://wiki.ros.org/navigation/Tutorials/RobotSetup) has been setup to implement autonomous navigation.

**File Descriptions**

- AGV_Motor_Control.ino is the Arduino code for motor control. The RPM control of motor is done through PWM inputs. Any motor can be used and controlled using this code by appropriately modifying the motor pin configurations

- src/ros_arduino.py file helps for ROS - Arduino communication with less latency.
The manual control of Mobile robot using direction keystrokes are possible with the help of src/agv_keyboard_control_ros.py file

- The files for performing Mapping, Localization, & Navigation are avilable in /launch directory

- Fine tune of path planning can be done by playing with the parameter files in /params directory 

- The Entire ROS nodes & topics used for this project can be visualised through the rosgraph.png file

- Libraries required for the successful implementation of this package are specified in file /ROS libraries for auto_nav

The video on this [link](http://wiki.ros.org/navigation/Tutorials/Using%20rviz%20with%20the%20Navigation%20Stack) will show the step by step instructions for implemeting navigation stack with the help of ROS visualization tool - RVIZ. 

With the use of this package Autonomous navigation of Mobile Robot from point A to B has been achieved. Further improvement has to be done by incorporating sensors like IMUs etc for odom improvement & by fine tuning or selecting suitable path planners which are application based.

Happy coding!


