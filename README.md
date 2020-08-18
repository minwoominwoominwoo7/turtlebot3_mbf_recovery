# turtlebot3_mbf_recovery  
  http://wiki.ros.org/move_base_flex  
  http://wiki.ros.org/move_base_flex/Tutorials  

# referenc git   
  https://github.com/uos/ceres_robot/tree/master/ceres_navigation  
  https://github.com/Rayman/turtlebot3_mbf  

# install   
sudo apt-get install ros-melodic-move-base-flex  
sudo apt-get install ros-melodic-py-trees  
sudo apt-get install ros-melodic-rqt-py-trees  
sudo apt-get install ros-melodic-py-trees-ros  
sudo apt-get install ros-melodic-sbpl-lattice-planner  
sudo apt-get install ros-melodic-eband-local-planner  
sudo apt-get install ros-melodic-rqt-smach  
sudo apt-get install ros-melodic-global-planner  

git clone https://github.com/minwoominwoominwoo7/turtlebot3_mbf_recovery  
git clone -b melodic-devel https://github.com/ros-visualization/executive_smach_visualization.git  
git clone https://github.com/uos/mbf_tools.git  
-> remove mbf_demo_controller folder   

# run  
roscore  
roslaunch turtlebot3_gazebo turtlebot3_world.launch  
roslaunch turtlebot3_mbf_recovery amcl_demo.launch   
rosrun turtlebot3_mbf_recovery navigation_sm.py  
rosrun smach_viewer smach_viewer.py  

# other state machine run  
rosrun turtlebot3_mbf_recovery mbf_future_planning.py  
rosrun turtlebot3_mbf_recovery mbf_move_base_action.py  
rosrun turtlebot3_mbf_recovery mbf_room_goal.py  
rosrun turtlebot3_mbf_recovery mbf_state_machine.py  