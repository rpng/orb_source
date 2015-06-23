# orb_source

This repo provides a simple hosting for launch files that create a video stream/sources for use in the [orb_slam](https://github.com/udel-robotics/orb_slam/) package. Launch files are located in the orb_launch folder and can be accessed in ROS Indigo by:

* roslaunch orb_launch gscam.launch
* roslaunch orb_launch asus-xtion.launch
* roslaunch orb_launch point-grey.launch


### Installation

This requires the gscam and openni2 package for ROS. The current install process is tested against ros Indigo.

1. Make sure you have installed ROS and all library dependencies.

2. Clone this repository to your catkin workspace:

  `git clone https://github.com/udel-robotics/orb_source.git orb_source`

3. Install needed dependencies for the gscam library:

  `sudo apt-get install libgstreamer0.10-dev libgstreamer-plugins-base0.10-dev`
  `sudo apt-get install libopenni2-dev`

4. Install needed dependencies for the point grey library:

  Install the latest FlyCapture drivers from http://www.ptgrey.com/downloads
  Note that you might have to install some dependencies
  Restart your computer after to ensure installation

5. Cd into the `orb_source` folder for dependency installation

6. Clone the needed libraries:

  * Gscam `git clone https://github.com/udel-robotics/gscam.git gscam`
  * Openni2 `git clone https://github.com/udel-robotics/openni2_camera.git openni2_camera`
  * Openni2 `git clone https://github.com/udel-robotics/openni2_launch.git openni2_launch`
  * Point Grey `git clone https://github.com/udel-robotics/pointgrey_camera_driver.git pointgrey_camera_driver`

7. Cd back to your home catkin workspace `cd ..`

8. Build your workspace with `catkin_make`

9. Configure your input source in the gscam.launch file.
  * Note that possible video feeds can be viewed here:
  * `ls /dev/video*`
