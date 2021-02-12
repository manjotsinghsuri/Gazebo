# Gazebo
Gazebo simulations and other things

## For using the Plugin, we need to build the package.

### For building the package, go to first_project folder.
'''
cd Simulations/first_project
'''

### Then create a folder named build there.
'''
mkdir build
'''

### Then inside build folder, build the package as done below
'''
cd build/
cmake ../
make
'''

### After that we need to set the path for the plugin to work
'''
export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/workspace/Simulations/first_project/build
'''


### Then launching the World in gazebo.
#### Go to world folder and then 
'''
gazebo submit_world6


