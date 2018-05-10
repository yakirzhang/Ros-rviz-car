# Ros-rviz-car
how to create a ros package named "car_simulation"
```
mkdir src
catkin_make
cd src
catkin_create_pkg car_simulation roscpp visualization_msgs
```
how to create a node "sim" In package car_simulation
```
add sim.cpp in src folder

// and then add following in CMakeLists.txt
add_executable(sim src/sim.cpp)
target_link_libraries(sim ${catkin_LIBRARIES})
```
