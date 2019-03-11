# Project: Build My World
A Gazebo world modeling my apartment, complete with some book cases and a couple of simple robots

## Installation
After cloning the repository to your local machine, navigate to the root folder and then run

```Bash
mkdir build # create build/ directory
cd build
cmake ../ # run cmake to create Makefile for welcome_message plugin
make # compile welcome_message plugin
export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:`pwd` # add newly-created build/ directory to Gazebo's plugin path
```

## Running the World
Once the plugin is compiled and added to Gazebo's plugin path, you can run this world with
```Bash
gazebo world/Apartment.world
```
from the root directory of this repository.

## Credits
Bookcase and table models included in the world come from Gazebo's online model library. The EmpressMobile is inspired by the "Make a Mobile Robot" tutorial at http://gazebosim.org/tutorials?tut=build_robot&cat=build_robot.
