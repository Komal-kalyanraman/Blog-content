while doing the tutorial "http://moorerobots.com/blog/post/2" when adding the range finder in my NON-GPU pc shadow was not being cast behind the placed obstrucles in the scene.

In the end of the blog it was written to replace libgazebo_ros_gpu_laser.so to libgazebo_ros_laser.so in file mybot.gazebo.

This alone will not solve the problem.

sensor type="gpu_ray" name="head_hokuyo_sensor" has to be changed to sensor type="ray" name="head_hokuyo_sensor"

the "gpu_ray" has to be changed to "ray" because this is a NON-GPU pc. The earlier .so will work fine for a GPU pc.
