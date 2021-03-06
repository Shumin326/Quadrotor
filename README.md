# Quadrotor

This  project is series of individual projects for the course "MEAM 620: Advanced Robotics" at Upenn. 

The project explores  a  quatrotor’s  capability  of maneuvering 3D space by designing an autonomy stack consisting  of  planning  and  control  algorithms.  Given a  3D  environment  map  with  obstacle  locations,  and,  a start and an end position, the goal is to fly a quadrotor smoothly  and  safely  from  start  to  end  based  on  the computed  trajectory.  The experiments are based on the CrazyFlie 2.0 robot which is quite small in size:

![](CrazyFlie.png)

- Control part is implementing the papers: “Minimum snap trajectory generation and control for quadrotors” from D. Mellinger and V. Kumar, and "Geometric tracking control of a quadrotor uav on SE(3)" from T. Lee, M. Leok, and N. McClamroch.

- graph search part uses Dijkstra and A* algorithm (implemented 2, but choose 1 to use) to generate collision free way points.

- trajectory is minimum-jerk quintic trajectory, it generates the actual path for quadrotors using the pruned way-points.

- lab results:
1. control test: fly a 1m cube

![](results/control_test.gif)

2. maze tests: fly from start to end point inside a maze, use graph search and min-jerk trajectory design. Here is the lab test video:

  - ![](results/maze_test.gif)
  
Also, the actual trajectory is recorded by vicon and we can compare it to the planned trajectory. 

The actual trajectory is in blue line, generated minimum jerk trajectory is in black line, original A* path is in red line.

  - ![](results/maze_test_1.png)

  - ![](results/maze_test_2.png)

  - ![](results/maze_test_3.png)
