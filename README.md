## Table Of Contents <a name="top"></a>

1. [New Robot Configuration](#1)
2. [Demo](#2) 
3. [Gazebo](#3)   
4. [Mapping](#4)    

 
  
 

## 1 New Robot Configuration <a name="1"></a>


- clone PURA_ROS_WS repository to your machine.



### Workspace Configuration
```bash
cd PURA_ROS_WS
```

```bash
rosdep install --from-paths src --ignore-src -r -y
```



## 3 Gazebo <a name="3"></a>
```bash
roslaunch pura_gazebo pura_gazebo.launch
```

## 4 Mapping <a name="4"></a>

Notes:

Please uncomment rviz line in pura_model.launch 

```bash

roslaunch pura_navigation pura_gmapping.launch
roslaunch pura_description pura_model.launch
rosrun map_server map_saver -f ~/<folder_name>/<map_name>
```


### Simulation
```bash
roslaunch pura_navigation pura_navigation.launch
```



