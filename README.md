# Gazebo Terrain Tutorial

A ros package to load a texture farmland with bumps for simulation in Gazebo.

## Installation

1. Clone this repository into the `src` in your ROS1 workspace

        $ cd /path/to/ros/workspace/src/
        $ git clone git@github.com:blackprince001/ros-farmland.git
        $ cd ../

2. Source the ROS system environment and source the Gazebo environment

        $ . /opt/ros/<ROS_DISTRO>/setup.bash
        $ . /usr/share/gazebo/setup.sh

3. Install dependencies and build the package

        $ rosdep install --from-paths src --ignore-src -r -y
        $ catkin_make

4. Source the workspace environment and launch the example

        $ . ./devel/setup.bash
        $ roslaunch ros-farmland farmland.launch

At this point, Gazebo should have launched and loaded the custom farmland. A common mistake is to forgot
to source the Gazebo environment in step 2.
