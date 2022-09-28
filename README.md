### Using Navvis Description package

This package has the model file for the Navvis robot. To use the file, write the following commands:
<br>
<code>
cd </package installation location> 
</code> <br>
<code>
source /opt/ros/noetic/setup.bash
</code> <br>
<code>
source devel/setup.bash
</code> <br>
<code>
catkin_make
</code> <br>
<code>
#Runs roscore in background
roscore &
</code> <br>
<code>
#Runs launcher that sets up relevant variables and uses urdf/xacro file to run rviz
</code> <br>
<code>
#Write this to run urdf file
</code> <br>
<code>
roslaunch rviz_config_launcher.launch &
</code> <br>
<code>
#Write this to run xacro file
</code> <br>
<code>
roslaunch rviz_config_launcher.launch use_xacro:=true &
</code> <br>
<code>
#Write this to opt out of running gui
</code> <br>
<code>
roslaunch rviz_config_launcher.launch use_gui:=false &
</code> <br>
<code>
#Rviz launches and shows file
</code>