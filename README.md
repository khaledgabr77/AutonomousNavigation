## Table Of Contents <a name="top"></a>

1. [Robot Configuration](#1)
2. [Gazebo](#2)   
3. [Mapping](#3)    
4. [Navigation](#4)    
5. [Referances](#5)    
6. [Result](#6)    


## 1 Robot Configuration <a name="1"></a>


- clone AutonomousNavigationAssignment- repository to your machine.


### Workspace Configuration
```bash
mkdir -p AutonomousNavigationAssignment/src
cd catkin_ws/src
git clone https://github.com/khaledgabr77/AutonomousNavigation.git
cd ..
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
roslaunch unit3_pp simulation_pura.launch

roslaunch unit3_pp unit3_astar_solution.launch 
```


## 5 Refrances <a name="5"></a>

https://brilliant.org/wiki/a-star-search/

https://www.101computing.net/a-star-search-algorithm/

http://wiki.ros.org/global_planner

http://wiki.ros.org/navigation/Tutorials/Writing%20A%20Global%20Path%20Planner%20As%20Plugin%20in%20ROS

http://wiki.ros.org/urdf/Tutorials

http://wiki.ros.org/gmapping

http://wiki.ros.org/move_base

https://github.com/rfzeg/path_planning_intro


## 6 Result <a name="6"></a>

# [Test video](https://www.youtube.com/watch?v=VtYBRn420Fw) 

