### Using Navvis Description package

This package has the model file for the Navvis robot. To use the file, write the following commands:
<code>
cd </package installation location>
source /opt/ros/noetic/setup.bash
source devel/setup.bash
catkin_make
#Runs roscore in background
roscore &
#Runs launcher that sets up relevant variables and uses urdf/xacro file to run rviz
#Write this to run urdf file
roslaunch rviz_config_launcher.launch  &
#Write this to run xacro file
roslaunch rviz_config_launcher.launch use_xacro:=true &
#Rviz launches and shows file
</code>