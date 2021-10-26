## Table Of Contents <a name="top"></a>

1. [Robot Configuration](#1)
2. [Gazebo](#2)   
3. [Mapping](#3)    
4. [Navigation](#4)    


## 1 Robot Configuration <a name="1"></a>


- clone AutonomousNavigationAssignment- repository to your machine.


### Workspace Configuration
```bash
mkdir -p AutonomousNavigationAssignment/src
cd AutonomousNavigationAssignment-
catkin_make
```

```bash
rosdep install --from-paths src --ignore-src -r -y
```



## 2 Gazebo <a name="2"></a>
```bash
roslaunch unit3_pp simulation_pura.launch
```

## 3 Mapping <a name="3"></a>

```bash

roslaunch pura_navigation pura_gmapping.launch
roslaunch pura_description pura_model.launch
rosrun map_server map_saver -f ~/<folder_name>/<map_name>
```


## 4 Navigation <a name="4"></a>

```bash
roslaunch unit3_pp unit3_astar_solution.launch 
```



