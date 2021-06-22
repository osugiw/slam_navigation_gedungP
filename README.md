# slam_navigation_gedungP
Final project of Artificial Intelligence in Automation and Robotics

by: 
- Miguel Lodewijk Jonas Luhulima  as 3D object designer, video designer 
- Sugiarto Wibowo                 as 3D object designer, map and world creator on Gazebo    
- Glenn Ricardo                   as 3D object designer, report writer              
- Jaselino Kevin                  as Simulator for SLAM and Navigation on Gazebo             


_info_:
- We are using turtlebot3 type burger

Prequisites:
1. Already install Virtualbox
2. Already install Ubuntu 18.04
3. Already install ROS-Melodic
4. Already install Gazebo
5. Already clone turtlebot3 or you can find out in this link (https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/)

How it works:
1. Create new package inside catkin_ws/src/ in this repository my folder name is **UAS_AI**
2. Inside UAS_AI there are 2 folder which is **launch** and **world**
3. 3D Model of gedung P are inside **world** folder, while **.launch** inside launch folder will be used for calling **.world**
4. Put the **model_editor_models** folder in home directory so Gazebo could initialized it

How I put object to gedung P world:
1. Make the gedung P by choosing **building editor** in Gazebo and import 2D Sketch of gedung P and draw the wall, etc.
2. Save the map in home directory by default location
3. Copy the folder that was made by making map to **catkin_ws/src/turtlebot3_simulations/turtlebot3_gazebo/models**
4. Open terminal by writing **sudo gazebo**, it is important to add sudo when you want to import object into models and save the worlds. In my case when I import the object to model without **Sudo** I couldn't save the world file
5. After that import gedungP model and import objects that we need


**notes:**
- All the objects was made in **Blender** and saved as .dae then import to Gazebo under /home/model_editor_models
- Always do catkin_make under catkin_ws/ after changing parameter or add files 


Some examples while we are trying the SLAM and Navigation:

![11](https://user-images.githubusercontent.com/51029305/122876972-4bfb1780-d360-11eb-9445-960483360645.png)
![22](https://user-images.githubusercontent.com/51029305/122876979-4e5d7180-d360-11eb-9aa3-a0adffcb61ba.png)
![33](https://user-images.githubusercontent.com/51029305/122876986-50273500-d360-11eb-97ff-06d4c1241073.png)
![44](https://user-images.githubusercontent.com/51029305/122876989-51586200-d360-11eb-8837-ea14a3c92b62.png)
![55](https://user-images.githubusercontent.com/51029305/122876992-51f0f880-d360-11eb-923c-93224b8be608.png)

