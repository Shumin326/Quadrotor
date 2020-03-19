# Quadrotor
- This project includes basically 4 parts: control, graph search, min-jerk trajectory design and lab. All of them are written in python.
- Control part is implementing papers: “Minimum snap trajectory generation and control for quadrotors” from D. Mellinger and V. Kumar, and "Geometric tracking control of a quadrotor uav on SE(3)" from T. Lee, M. Leok, and N. McClamroch.
- graph search part uses Dijkstra and A* algorithm (implemented 2, but choose 1 to use) to generate collision free way points.
- trajectory is minimum-jerk(5th order), it generates the actual path for quadrotors using the pruned way-points.
