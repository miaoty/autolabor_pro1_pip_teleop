#autolabor_pro1_pip_teleop

车体gazebo开启：
```shell
roslaunch autolabor_gazebo_worlds autolabor_pro1_gazebo.launch    #车体
roslaunch autolabor_gazebo_worlds autolabor_pro1_rplidar_gazebo.launch     #车体+rplidarA1
roslaunch autolabor_gazebo_worlds autolabor_pro1_rslidar16_gazebo.launch     #车体+rslidar16
```

键盘控制(cmd/vel)： 
```shell
roslaunch autolabor_pro1_teleop autolabor_pro1_teleop.launch # i j l ,
```
手柄控制(cmd/vel)： 
```shell
roslaunch teleop_twist_joy teleop.launch    #LB+RB+left 直观看手柄响应：sudo jstest /dev/input/js* http://wiki.ros.org/joy/Tutorials/ConfiguringALinuxJoystick  
```
车体驱动：
```shell
roslaunch autolabor_pro1_driver driver.launch
```
slam:
navigation:ff

piping_description：solidworks生成的urdf

reference:  https://github.com/kinglintianxia/autolabor_pro1
