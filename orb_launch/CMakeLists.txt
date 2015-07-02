cmake_minimum_required(VERSION 2.8.3)
project(orb_launch)

find_package(catkin)

catkin_package(
  CATKIN_DEPENDS
    gscam
    openni2_camera
    openni2_launch
)