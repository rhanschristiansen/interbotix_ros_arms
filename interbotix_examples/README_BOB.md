# Running the wx200 robot arm with Moveit
## Quickstart
Use the following command from `interbotix_ws/interbotix_examples` directory:
```bash
roslaunch interbotix_moveit_interface moveit_interface.launch robot_name:=wx200 use_cpp_interface:=true use_actual:=true use_python_interface:=true
```
## Custom pose for start/goal states
Under `MotionPlanning->Planning Request` select the Query Start State and Query Goal State checkboxes. You should now be able to select `Interact` in the top left corner and click/drag the robot into various orientations.
