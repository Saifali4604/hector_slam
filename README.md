# hector_slam
creating the directory/ workspace
```
mkdir -p ~/rplidar/src
cd ~/rplidar/src
```
git cloning
```
cd ~/rplidar/src
git clone https://github.com/Saifali4604/hector_slam
git clone https://github.com/robopeak/rplidar_ros
```
open file manager and open rplidar/src and extract the hector_slam file
delete the zip file
then follow the below cmds

```
cd ..
catkin_make
source ~/rplidar/devel/setup.bash
gedit ~/.bashrc
```
paste the below line at the bottom
```
source ~/rplidar/devel/setup.bash
```
plug the RPLIDAR to the system
```
ls -l /dev |grep ttyUSB
sudo chmod 666 /dev/ttyUSB0
```
use below cmds to run rplidar and view the output without hector slam
```
roscore
roslaunch rplidar_ros view_rplidar.launch
```
use below cmds to run rplidar and view the output with hector slam
```
roscore
roslaunch rplidar_ros rplidar.launch
roslaunch hector_slam_launch tutorial.launch
```



