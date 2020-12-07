# iai_donbot_ws
Follow these steps:
```
source /opt/ros/melodic/setup.bash          # start using ROS melodic
mkdir -p ~/iai_donbot_ws/src                # create directory for workspace
cd ~/iai_donbot_ws/src                      # go to workspace directory
wstool init                                 # init rosinstall
wstool merge https://raw.githubusercontent.com/K4R-IAI/iai_donbot_ws/master/iai_donbot.rosinstall
                                            # update rosinstall file
wstool update                               # pull source repositories
cd ..                                       # go to workspace directory
rosdep install --from-paths src --ignore-src -r -y    # install missing packages
catkin_make                                 # build packages
source ~/iai_donbot_ws/devel/setup.bash     # source new overlay
```
## Prerequisites:
Ubuntu 18.04
Unreal Engine 4.22.3
