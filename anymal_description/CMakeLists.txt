cmake_minimum_required(VERSION 3.0.0)
project(anymal_description)

find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY meshes/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/meshes
  PATTERN ".svn" EXCLUDE)

install(DIRECTORY robots/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/robots
  PATTERN ".svn" EXCLUDE)

install(DIRECTORY params/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/params
  PATTERN ".svn" EXCLUDE)
