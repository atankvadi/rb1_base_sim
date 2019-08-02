cmake_minimum_required(VERSION 2.8.3)
project(rb1_base_stage)


find_package(catkin REQUIRED)


catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES rb1_base_stage
#  CATKIN_DEPENDS other_catkin_pkg
#  DEPENDS system_lib
)

#############
## Install ##
#############

## Mark other files for installation (e.g. launch and bag files, etc.)
install(DIRECTORY
   rviz
   world
   launch
   DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
