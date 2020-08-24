# iai_donbot_ws
Follow these steps:
```
source /opt/ros/melodic/setup.bash          # start using ROS melodic
mkdir -p ~/iai_donbot_ws/src                # create directory for workspace
cd ~/iai_donbot_ws/src                          # go to workspace directory
wstool init                                 # init rosinstall
wstool merge https://github.com/K4R-IAI/iai_donbot_ws/commit/6bfc38c5cd6611d5a2d7061455334b7ca9aea519
                                            # update rosinstall file
wstool update                               # pull source repositories
cd ..                                       # go to workspace directory
catkin_make                                 # build packages
source ~/iai_donbot_ws/devel/setup.bash     # source new overlay
```
## Prerequisites:
Ubuntu 18.04  
Unreal Engine 4.22.3
