# hector_slam
creating the directory/ workspace
```
mkdir rplidar
cd rplidar
mkdir src
cd src
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
source ~/catkin_ws/devel/setup.bash
```
plug the RPLIDAR to the system
```
ls -l /dev |grep ttyUSB
sudo chmod 666 /dev/ttyUSB0
```

