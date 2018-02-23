## Overview

This is the code for the ARIAC (http://gazebosim.org/ariac)  qual1a, which required the arm grap two rods, three grears and place them 
in the tray one by one. This is done by programmatically interface with the ROS interface that is used to interact with the ARIAC competition simulation.
The main idea of this code is: read the order geiven by the config file, and then move the arm along a hand code trajector. Grab the part
when it close to the desired bin and place the part to the desired tray.

## Future Work
Another way will be created using MoveIt! interface later. So that the planning part will be handled by planning library with MoveIt!


## Build and Run
```
git clone https://github.com/zzjkf2009/ARIAC_Qual1a_Zejiang
cd <path_to_this_workspace>
catkin_make
rosrun osrf_gear gear.py -f `catkin_find --share osrf_gear`/config/qual1a.yaml <path_to_your_config_file>.yaml
rosrun ariac_example ariac_example_node
```


