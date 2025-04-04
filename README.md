# Universal Robot

[ROS-Industrial](https://wiki.ros.org/Industrial) Universal Robot meta-package. See the [ROS wiki](https://wiki.ros.org/universal_robots) page for compatibility information and other more information.

__License__

The [UR20 meshes](ur_description/meshes/ur20) and [UR30 meshes](ur_description/meshes/ur30) constitute “Graphical Documentation” from Universal Robots which is subject to and governed by Universal Robots' "[Terms and Conditions for use of Graphical Documentation](https://www.universal-robots.com/legal/terms-and-conditions/terms_and_conditions_for_use_of_graphical_documentation.txt)".

Universal Robots' [Terms and Conditions for use of Graphical Documentation](https://www.universal-robots.com/legal/terms-and-conditions/terms_and_conditions_for_use_of_graphical_documentation.txt) do not fully comply with [OSI's definition of Open Source](https://opensource.org/osd/), but they do allow you to use, modify and share “Graphical Documentation”, including [UR20 meshes](ur_description/meshes/ur20) and [UR30 meshes](ur_description/meshes/ur30), subject to certain restrictions.\
If you have any questions regarding this license or if this license doesn't fit your use-case, please contact [legal@universal-robots.com](mailto:legal@universal-robots.com).

All other content is licensed under the BSD-3-Clause license or Apache-2.0 respectively.

---

In the following the commands for the UR10e are given. 

For setting up the MoveIt! nodes to allow motion planning run e.g.:

```roslaunch ur10e_moveit_config moveit_planning_execution.launch```

For starting up RViz with a configuration including the MoveIt! Motion Planning plugin run:

```roslaunch ur10e_moveit_config moveit_rviz.launch```

___Usage with Gazebo Simulation___
There are launch files available to bringup a simulated robot.

Don't forget to source the correct setup shell files and use a new terminal for each command!

To bring up the simulated robot in Gazebo, run:

```roslaunch ur_gazebo ur10e_bringup.launch```


___MoveIt! with a simulated robot___
Again, you can use MoveIt! to control the simulated robot.

For setting up the MoveIt! nodes to allow motion planning run:

```roslaunch ur10e_moveit_config moveit_planning_execution.launch sim:=true```

For starting up RViz with a configuration including the MoveIt! Motion Planning plugin run:

```roslaunch ur10e_moveit_config moveit_rviz.launch```
