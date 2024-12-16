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
- 
## SLAM algorithm 

## Results with somulated data
<img width="874" alt="image" src="https://github.com/user-attachments/assets/a9cf73ab-e22c-45e7-8c04-69df4f597606" />


## Results with real data 
<img width="1201" alt="Снимок экрана 2024-12-17 в 00 33 40" src="https://github.com/user-attachments/assets/bee40fca-da35-484a-9296-83ed19a06389" />
