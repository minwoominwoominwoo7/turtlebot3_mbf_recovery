cmake_minimum_required(VERSION 2.8.3)
project(turtlebot3_mbf_recovery)

find_package(catkin REQUIRED COMPONENTS
  rospy
)

################################################################################
# Setup for python modules and scripts
################################################################################
catkin_python_setup()

###################################
## catkin specific configuration ##
###################################

catkin_package(
  CATKIN_DEPENDS rospy
)


#############
## Install ##
#############

#catkin_install_python(PROGRAMS
#  scripts/test.py
#  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
#)

#install(DIRECTORY launch
#  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
#)



