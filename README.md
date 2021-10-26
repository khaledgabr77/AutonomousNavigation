## Table Of Contents <a name="top"></a>

1. [New Robot Configuration](#1)
2. [Gazebo](#2)   
3. [Mapping](#3)    

 
  
 

## 1 New Robot Configuration <a name="1"></a>


- clone AutonomousNavigationAssignment- repository to your machine.


### Workspace Configuration
```bash
cd AutonomousNavigationAssignment-
catkin_make
```

```bash
rosdep install --from-paths src --ignore-src -r -y
```



## 2 Gazebo <a name="3"></a>
```bash
roslaunch unit3_pp simulation_pura.launch
```

## 3 Mapping <a name="4"></a>

```bash

roslaunch pura_navigation pura_gmapping.launch
roslaunch pura_description pura_model.launch
rosrun map_server map_saver -f ~/<folder_name>/<map_name>
```






