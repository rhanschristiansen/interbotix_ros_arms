# Running the wx200 robot arm with Moveit
## Quickstart
Use the following command from `interbotix_ws/interbotix_examples` directory:
```bash
roslaunch interbotix_moveit_interface moveit_interface.launch robot_name:=wx200 use_cpp_interface:=true use_actual:=true use_python_interface:=true
```
## Custom pose for start/goal states
Under `MotionPlanning->Planning Request` select the Query Start State and Query Goal State checkboxes. You should now be able to select `Interact` in the top left corner and click/drag the robot into various orientations.

## Installing ROS on Ubuntu 18.04
If you are on a new machine without ROS installed, install the following:
```bash
sudo bash
sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
apt-get update
apt install ros-melodic-ros-base
apt install ros-melodic-desktop
source /opt/ros/melodic/setup.bash
```
