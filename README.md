# Gazebo
Gazebo simulations and other things

## Table Of Contents
- [Project 1](Project-1)
- [Project 2](Project-2)

## Project 1
---
## For using the Plugin, we need to build the package.

* For building the package, go to first_project folder.

    `cd Simulations/first_project`

* Then create a folder named build there.

    `mkdir build`


* Then inside build folder, build the package as done below

    ```
    cd build/
    cmake ../
    make
    ```


* After that we need to set the path for the plugin to work

    `export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/workspace/Simulations/first_project/build`

### Then launching the World in gazebo.

* Go to world folder and then 

    `gazebo submit_world6`

## Project 2
---

There are 2 packages :
* my_robot - Launching the world and the URDF model
* ball_chaser - Launching 2 nodes for following the white ball

1. First source the packages in the terminal

    `cd workspace`

    `source devel/setup.bash`
2. Then launch the my_world.launch launch file

    `roslaunch my_robot my_world.launch`

3. Then launch the ball_chaser.launch launch file

    `roslaunch ball_chaser ball_chaser.launch`

4. Now set the rviz configuration so that you can see camera images, robotmodel and lasercscan

5. Now move the white ball in the gazebo so as to make the robot model follow the white ball