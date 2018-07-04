# Rowbot 

Sydney University Team 
Robotx Challenge 2018

## Description

This is a simulation stack for the Rowbot team. It includes Kingfisher and Wam-V robot descriptions, training worlds, to allow software development.

## Use

```sh
roslaunch robotx_gazeo sandisland.launch
# Or with parameters
roslaunch robotx_gazeo sandisland.launch usv:=kingfisher world:=ocean_buoys.world
```

| Name  	| Values                                                    	| Description                   	|   	|
|-------	|-----------------------------------------------------------	|-------------------------------	|---	|
| usv   	| kingfisher wamv                                           	| The robot model to work with  	|   	|
| world 	| ocean_buoys.world sandisland_buoys.world sandisland.world 	| World description                        	|   	|

## Sources

Most of `wamv_description` and `robotx_gazebo` come from the official `osrf/vmrc` Mercurial repository (https://bitbucket.org/osrf/vmrc), and are developped for te Virtual Maritime Challenge.

They included the sources of the `usv_gazebo_plugins` inside for practical reasons (these can be find at https://github.com/bsb808/usv_gazebo_plugins).

The `kingfisher_description` is an extension of the Clearpath's official URDF description (accessible at https://github.com/kf/kingfisher).

## Dependencies

Tested platform : Ubuntu 16.04 LTS, ROS Kinetic Kame, Gazebo 7

### Velodyne Simulator

Gazebo plugin to simulate Gazebo LIDAR. 

https://bitbucket.org/DataspeedInc/velodyne_simulator/

### URDF tutorials

Optionnal dev depedency. 
Used to check the consistency of URDF descriptions

