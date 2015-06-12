# gscam_launch

This repo provides a simple hosing for launch files that create a video stream for use in the [orb_slam](https://github.com/udel-robotics/ORB_SLAM) package. Launch files are located in the launch folder and can be accessed in ROS Indigo with the command `roslaunch gscam_launch webcam.launch`.

### Installation

This requires the gscam package for ROS. The current install process is tested against ros Indigo.

1. Make sure you have installed ROS and all library dependencies.

2. Clone this repository to your catkin workspace:
  `git clone https://github.com/udel-robotics/gscam_launch.git gscam_launch`

3. Install needed dependencies for the gscam library:
  `apt-get install libgstreamer0.10-dev libgstreamer-plugins-base0.10-dev`

4. Clone the gscam library:
    `git clone https://github.com/udel-robotics/gscam.git gscam`

5. Build your workspace with `catkin_make`

6. Configure your input source in the .launch file.
  * Note that possible video feeds can be viewed here:
  * `ls /dev/video*`




