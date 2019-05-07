# marvin_moveit

This package is the [MoveIt!](http://moveit.ros.org) implementation for the Jaco arm on Marvin. Almost all the files inside this package
are generated by the [MoveIt! Setup Assistant] (http://docs.ros.org/kinetic/api/moveit_tutorials/html/doc/setup_assistant/setup_assistant_tutorial.html).

This package is depended on the on the marvin_gazebo and marvin_sim_package package, therefore it must be launched beforehand in a separate terminal.

`roslaunch marvin_gazebo marvin_world.launch`

**To launch this package:**

`roslaunch marvin_moveit demo.launch`

Once you launch this package, pre-configured Rviz will open up with the Motion Planning display that you can use to specify the start and end poses
for the Marvin_Jaco. Then you can click on `Plan` to visualise the planning and then `Execute` for the Marvin to execute the planned trajectory.

`roslaunch marvin_moveit test_sim.launch`

Once you launch this package, pre-configured Rviz will open up with the Motion Planning display that you can use to specify the start and end poses
for the Marvin_Jaco.And also controls the marvin_gazebo and can be configured to marvin_hardware interaction with moveit_rviz

On Sucessfullly Launching the marvin_moveit Package.

![Marvin_Moveit](marvin_moveit/Move_it_rvZ_Marvin.png)

**Possible Issues:**

- none

**prerequisites:**

`sudo apt-get install ros-kinetic-moveit`        (ensure that it's installed on your system before launching moveit)

`sudo apt-get install ros*controller*` (Install the Necessary Controllers for the Gazebo and ROS)