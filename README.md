# Robot Programming Assesment 

## Using this code - update the file 
```bash
colcon build --symlink-install

source install/setup.bash
```
## 1.Using this command to run the world in Gazebo
### 1.1 For running the default Gazebo world 
```bash
ros2 launch limo_gazebosim limo_gazebo_diff.launch.py
```
### 1.2 For running my world(saved world)
```bash
ros2 launch limo_gazebosim limo_gazebo_diff.launch.py world:=src/cmp9767_tutorial/worlds/my_testworld.world
```

## 2.Using this command to run the navigation 
### 2.1 For running the defauft map 
```bash
ros2 launch limo_navigation limo_navigation.launch.py
```
### 2.2 For running my map (saved map)
```bash
ros2 launch limo_navigation limo_navigation.launch.py map:=src/cmp9767_tutorial/maps/my_map.yaml use_sim_time:=true
```
##