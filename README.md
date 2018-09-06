# Pioneer P3-AT

In order to use it:

Add to your gazevo path the "cic" folder that is inside the "world" folder(copy here):
	cd ~/.gazebo/models

you can easy move it with
rostopic pub -1 /cmd_vel geometry_msgs/Twist '[0.5, 0.0, 0.0]' '[0.0, 0.0, 0.0]'

DEMO WITHOUT MAP:
In two separate terminal windows:
    Start the Pioneer 3AT simulation environment:
        roslaunch pioneer pioneer3at.gazebo.launch

    Start the move_base demo:
        roslaunch pioneer move_base_mapless_demo.launch

DEMO LOCALIZATION WITH MAP:
In two separate terminal windows:
    Start the Pioneer 3AT simulation environment:
        roslaunch pioneer pioneer3at.gazebo.launch

     Start the amcl demo:
        roslaunch pioneer amcl_demo.launch
        
        

