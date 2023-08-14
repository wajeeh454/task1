# SM23-AI-ROS-01
Installing full Smart-Methods Ros packages for robot arm
# Installing process
1- Install Virtual Box (https://www.virtualbox.org/wiki/Downloads)

2- Install ubuntu 18.04 version (/https://releases.ubuntu.com/18.04)

3- Open Virtual Box, click new, select VB Name (Name: ROS_Naif)
# Process of ROS installation inside ubuntu
1- Select Terminal inside ubunto then follow the given instructions on (https://wiki.ros.org/)

2- Our compatible version of ROS on ubuntu 18.04 is ROS melodic
# ROS melodic installation commands guide in ubuntu terminal by order:
1) sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

2) sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

3) sudo apt-get update

4) sudo apt-get install ros-melodic-desktop-full

5) echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
source ~/.bashrc

6) sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential

7) sudo apt install python-rosdep

8) sudo rosdep init

9) rosdep update

10) source /opt/ros/melodic/setup.bash

11) Creating a workspace for catkin:

mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

12) cd ~/catkin_ws/src

13) sudo apt install git

14) git clone https://github.com/smart-methods/arduino_robot_arm 

15) cd ~/catkin_ws

16) rosdep install --from-paths src --ignore-src -r -y

17) sudo apt-get install ros-melodic-moveit

18) sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui

19) sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher

20) sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control

21) Compile the package:

 catkin_make

23) Lunch ROS:

roslaunch robot_arm_pkg check_motors.launch
# Resources used to download ROS:
1) Smart-Methods installation commands of ROS (https://s-m.com.sa/ros.txt)
2) Ubuntu install of ROS packages(http://packages.ros.org/ros/ubuntu)
3) Creating a workspace for catkin (http://wiki.ros.org/catkin/Tutorials/create_a_workspace)
4) Ubuntu install of ROS Melodic (http://wiki.ros.org/melodic/Installation/Ubuntu)
# Tutorials of ROS packages after installation:
1) Package Summary Tutorials (http://wiki.ros.org/rviz)
