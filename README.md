#Aritra Question 2 by NA22B051
The repository consists of three parts: URDF_models, Vessel_ctrl_setup, and media.

#Integration with RVIZ2:
1. Ensure the requirements are installed and URDF files are downloaded.
2. To visualize the KCS dummy model in RVIZ2, run "ros2 launch urdf_tutorial display.launch.py model:=/pathtofile/kcs_model.urdf".
3. To visualize the otter catamaran dummy model in RVIZ2, run "ros2 launch urdf_tutorial display.launch.py model:=/pathtofile/otter_katamaran_model.urdf".
#ROS2 Control Setup:
1. Make sure the requirements are installed, and the vessel_ctrl_setup folder is downloaded.
2. Two nodes are available: "kcs_ctrl" and "otter_ctrl".
3. Watch the demo video of KCS control in the /media folder.
4. Run "ros2 run week_2 kcs" in terminal 1.
5. Run "ros2 run teleop_twist_keyboard teleop_twist_keyboard" in terminal 2.
6. Run "ros2 run vessel_ctrl_setup kcs_ctrl" in terminal 3.
7. To observe changes, execute "ros2 topic echo /kcs/odom". (Note: "ros2 topic list" showed /kcs/odom, not /kcs/kcs/odom, so the same will reflect in the node file "/kcs/commands".)
