# ROS2-study

1. Activate ROS2:
cd C:\dev\lyrical\ros2-windows
pixi shell
set ROS_DOMAIN_ID=0
set QT_QUICK_BACKEND=software
.\local_setup.bat

2. Turn on turtlesim:
Activate ROS2
ros2 run turtlesim turtlesim_node

Open a new terminal
Activate ROS2
ros2 run turtlesim turtle_teleop_key

3. To turn on rqt:
Open a new terminal
Activate ROS2
.\\local_setup.ps1
rqt

4. To control 2nd turtle:
Open a new terminal
Activate ROS2
cmd
call setup.bat
ros2 run turtlesim turtle_teleop_key --ros-args --remap turtle1/cmd_vel:=turtle2/cmd_vel
