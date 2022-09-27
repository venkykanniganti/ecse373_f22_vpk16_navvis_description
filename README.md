### Using Navvis Description package

This package has the model file for the Navvis robot. To use the file, write the following commands:
<br>
<code>
cd </package installation location> 
</code> <br>
<code>
source /opt/ros/noetic/setup.bash<br>
source devel/setup.bash<br>
catkin_make<br>
#Runs roscore in background<br>
roscore &<br>
#Runs launcher that sets up relevant variables and uses urdf/xacro file to run rviz<br>
#Write this to run urdf file<br>
roslaunch rviz_config_launcher.launch  &<br>
#Write this to run xacro file<br>
roslaunch rviz_config_launcher.launch use_xacro:=true &<br>
#Rviz launches and shows file<br>
</code>