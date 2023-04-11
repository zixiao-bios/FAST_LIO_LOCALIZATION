cmake_minimum_required(VERSION 2.8.3)
project(fast_lio_localization)

catkin_package(
  CATKIN_DEPENDS geometry_msgs nav_msgs roscpp rospy std_msgs message_runtime
  DEPENDS
  INCLUDE_DIRS
)

catkin_install_python(PROGRAMS scripts/global_localization.py scripts/transform_fusion.py
                      DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})