# 4WheelDrive-LIDAR_Gazebo
The repo contains a description folder which has files necesary for simulating a 4-wheeled differential skid steer drive robot in Gazebo. Src folder contains launch, urdf and mesh files. Universal Robot Description File (URDF) contains XACRO files necessary for describing joint and link parameters, while launch files contain display parameters for both RVIZ and Gazebo. The folder has been generated after creating a model in fusion 360 and converting it using URDF exporter.
## Distribution and Packages
Please note that ROS1 with melodic distribution has been used. Kindly alter your packages according to the distribution being used.
Gazebo tags for LIDAR and Skid-steer have been added in the gazbeo.launch file. Edit that file for addition/removal of tags. 
## Running the robot simulation 
To launch the gazebo file, initiate a catkin workspace in ROS. Inside src folder, add the mybody_description folder. 

For Gazebo, run : **roslaunch mybody_description gazebo.launch**

For RVIZ Visualization, run: **roslaunch mybody_description display.launch**

## Pre-requisites 
Note that you require a build tool (catkin in this case) and ros distribution to run these files. Gazebo must be installed, which you can do from [here](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwi5peby9siDAxWOxgIHHToVD7YQFnoECBIQAQ&url=https%3A%2F%2Fclassic.gazebosim.org%2Ftutorials%3Ftut%3Dinstall_ubuntu&usg=AOvVaw2pD1-zHYHUQ2AOo8zHRB5s&opi=89978449). I have used Gazebo 9 version for the ske of this project

