# Gazebo Package for BetaGo 
This is gazebo package for BetaGo.

## File explanation
This section is used to explain what some files do.
- launch/betago/betago_world.launch: load BetaGo in gazebo.
- launch/betago/rviz_control_gazebo.launch: view the BetaGo in rviz and control the BetaGo to move in the gazebo, so launch the betago_world.launch then launch this node.

## start betago_world
```
cd ~/BetaGo_ws
source devel/setup.sh 
roslaunch betago_gazebo betago_world.launch
```

## start rviz_control_gazebo 
```
cd ~/BetaGo_ws
source devel/setup.sh 
roslaunch betago_gazebo rviz_control_gazebo.launch
```

## Control betaGo with keyboard
```
sudo apt-get install ros-melodic-teleop-twist-keyboard
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

## Notes
ros_control is loaded in ridgeback.gazebo which is included by ridgeback.urdf.xacro

## Modify on other project used in BetaGo
None
