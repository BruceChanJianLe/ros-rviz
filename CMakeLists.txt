cmake_minimum_required(VERSION 3.0.2)
project(ros-rviz)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  rviz
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES ros-rviz
#  CATKIN_DEPENDS roscpp rospy rviz
#  DEPENDS system_lib
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)
