# SLAM-system-for-Geodata

## Dataset link
https://drive.google.com/drive/folders/1A5l76n0dPEYNBwRk_kqAiJ8qz0d5BfQJ?usp=share_link 
https://projects.asl.ethz.ch/datasets/doku.php?id=kmavvisualinertialdatasets

## Description 

This project implements a 3D Particle Filter-based Simultaneous Localization and Mapping (SLAM) algorithm. The system simulates a quadcopter navigating through a labyrinth-like environment, using RGB and depth images as sensor inputs. The algorithm estimates the quadcopter's trajectory and builds a 3D occupancy grid map of the environment.

The key components of the system include:

- **Particle Filter**: A probabilistic method for estimating the quadcopter's pose using a set of particles.
- **Occupancy Grid Map**: A 3D grid representing the environment, where each cell indicates the presence or absence of obstacles.
- **Sensor Model**: A probabilistic model that updates particle weights based on simulated sensor measurements.
- **Motion Model**: A model that predicts the quadcopter's movement based on control inputs and adds noise to simulate real-world conditions.
## SLAM algorithm 

The slam function is the core of the SLAM (Simultaneous Localization and Mapping) algorithm. It integrates all the components of the particle filter-based SLAM system, including particle initialization, motion modeling, sensor modeling, resampling, map updates, and visualization. The function simulates the quadcopter's navigation through a 3D labyrinth environment, estimating its trajectory and building a 3D occupancy grid map.

The slam function takes the following parameters:

- **num_iterations (int)**: The number of iterations (time steps) to run the SLAM algorithm. FE 20 (run the algorithm for 20 time steps).
- **control_inputs** (list of numpy arrays): A list of control inputs for each iteration. Each control input is a 3D vector representing the movement in the X, Y, and Z directions.
FE [np.array([0.1, 0.2, 0.0]), np.array([0.3, 0.1, 0.0]), ...] (a list of control inputs for each iteration).

## Results with somulated data
<img width="874" alt="image" src="https://github.com/user-attachments/assets/a9cf73ab-e22c-45e7-8c04-69df4f597606" />


## Results with real data 
<img width="872" alt="image" src="https://github.com/user-attachments/assets/2fe1c1c9-fbf0-4b0e-824a-d92ba1b5815a" />
<img width="872" alt="Снимок экрана 2024-12-17 в 00 33 40" src="https://github.com/user-attachments/assets/bee40fca-da35-484a-9296-83ed19a06389" />
