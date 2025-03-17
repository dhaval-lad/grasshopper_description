# grasshopper_description

## Description
![GrassHopper Robot](meshes/GrassHopper)

The `grasshopper_description` ROS2 package for simulating a 4-WD robot called "GrassHopper". The simulated robot consist of 2D-Lidar, Depth Camera, and IMU sensor plugin. 

## Dependencies
- ROS2

## Installation Instructions
1. First, clone this repository inside the `src` folder of your ROS 2 workspace (replace `ros2_ws` with the name of your ROS 2 workspace):
    ```sh
    cd ~/ros2_ws/src
    git clone https://github.com/dhaval-lad/grasshopper_description.git
    ```
2. Change the path of the mesh file in `grass_hopper.urdf.xacro`. Mesh files are located in `meshes`folder inside the package. Replace path with the path on your system in lines (56, 91,99,131,139,175,183,219,227,263,271).
3. Next, build your ROS 2 workspace to install the package (replace `ros2_ws` with the name of your ROS 2 workspace):
    ```sh
    cd ~/ros2_ws
    colcon build --packages-select grasshopper_description
    ```

## Usage Instructions
To verify that everything is working:
1. Run the following command in the terminal to visualize the GrassHopper robot in RViz2:
    ```sh
    ros2 launch grasshopper_description description.launch.py 
    ```

## Contributors  

We extend our gratitude to the incredible contributors who played a vital role in bringing the GrassHopper robot to life:  

- **[Mayank Khandelwal](https://github.com/itsMayankKhandelwal)** – Crafted detailed and precise mesh files for every component of the GrassHopper robot, laying the foundation for realistic visualization and simulation.  

- **[Dhaval Lad](https://github.com/dhaval-lad)** – Developed the **`grasshopper_description`** ROS2 package, enabling seamless simulation of the GrassHopper robot in Gazebo and bringing it one step closer to real-world deployment.  

## License
This project is licensed under the Apache License, Version 2.0, January 2004. See [http://www.apache.org/licenses/](http://www.apache.org/licenses/) for more details.