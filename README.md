# Task-3-Using-another-ROS-robot-with-SLAM-approach-to-create-and-save-a-map
I was able to complete this task from the help of the telegram group - spichal thankes to [mo7ammed-saleh](https://github.com/mo7ammed-saleh) for shearing his repositories gethub in the telegram group.

# HOW TO USE ANOTHER ROSROBOT FOR THE TASK
1.the steps to installing the ROSbot
similar to mohammad i took Refrences from [Amg0z](https://github.com/Amg0z/warehouse_simulation_toolkit/blob/master/README.md) and followed his steps

The steps i followed:
1.Downloading the ROS package using: 
```
sudo apt-get install ros-melodic-hector-trajectory-server ros-melodic-slam-gmapping ros-melodic-navigation
```

2.Installing the Build:
  2.1.first we clone the repository using:
  ```
    cd ~/catkin_ws/src
    git clone https://github.com/wh200720041/warehouse_navigation.git
    cd ..
    catkin_make
    source ~/catkin_ws/devel/setup.bash
  ```
  in the terminal

  2.2.Then lunch ROS using:
  
```
    roslaunch warehouse_simulation warehouse_simulation.launch
```
After lunching ros these two aplicatios will start(gazebo,Rviz)

# SHOWING THE TWO APLICATION THAT WILL START
![CaPture (2)](https://user-images.githubusercontent.com/85543378/126920882-2d65bff4-2004-4130-b4b1-f94146366512.JPG)
  3.Controling the similation there are two ways to control
  3.1.we can control the similation using the keyboard arrows in the terminal.
  
  3.2.Or we can you the [♐2D Nav Goal] icon in the Rviz similation
  and that what i personally used for the ease of use.
  
# SHOWING HOW TO CONTROL THE ROBOT IN THE SIMILATION
  ![ezgif-3-a2983eccedb1](https://user-images.githubusercontent.com/85543378/126921262-671a7cc0-62bf-4d1a-a51e-4a73b50b7697.gif)

4.Saving the similation map
4.1. We save the similation map by using this code `rosrun map_server map_saver -f ~/map` in a new terminal to save a photo of the similation map

## PHOTO OF THE SAVED MAP
![zzz](https://user-images.githubusercontent.com/85543378/126922297-a5c8b225-7def-4c53-bca7-e1c3f89c854b.JPG)
