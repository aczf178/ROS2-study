# ROS2-study

## Activate ROS2:

cd C:\dev\lyrical\ros2-windows

pixi shell

set ROS_DOMAIN_ID=0

set QT_QUICK_BACKEND=software

.\local_setup.bat


## Turn on turtlesim:
### 1. turtlesim_node

**Activate ROS2**

ros2 run turtlesim turtlesim_node

### 2. turtle_teleop_key

Open a new terminal

**Activate ROS2**

ros2 run turtlesim turtle_teleop_key


## To turn on rqt:

Open a new terminal

**Activate ROS2**

.\\local_setup.ps1

rqt



## To control 2nd turtle:

Open a new terminal

**Activate ROS2**

cmd

call setup.bat

ros2 run turtlesim turtle_teleop_key --ros-args --remap turtle1/cmd_vel:=turtle2/cmd_vel
