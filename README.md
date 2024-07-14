# A Statistical Similarity Measure for Aggregate Crowd Dynamics
- Packages to install:
  (i) ultralytics (to import YOLOv8n model)
  (ii) OpenCV

## Objective:
• To develop comprehensive crowd simulation models to accurately simulate and predict pedestrian dynamics, enhance urban safety and optimize crowd management

## Approach:
1) Data Collection and Preprocessing: Utilized YOLOv8n for tracking pedestrian movements in video footage with detection accuracy of 92%. Extracted positional and velocity data to create a comprehensive dataset for simulation.

2) Ensemble Kalman Smoothing (EnKS): Utilized EnKS to estimate and refine pedestrian state distributions, improving the tracking accuracy by 15%.

3) Model Implementation:
(i) Steering Model: Implemented the Steering Model to guide pedestrian movements based on a set of behavioral rules and forces.
(ii) Social Force Model: Simulated realistic pedestrian interactions and movements based on social forces, considering factors like personal space and social interactions.
(iii) Predictive Planning Model: Applied Reciprocal Velocity Obstacle (RVO) for collision avoidance and optimal path planning, using linear programming to compute optimal velocities for agents.

4) Validating Model Accuracy: Calculated metrics such as entropy, error mean, & error standard deviation using Maximum Likelihood Estimation to evaluate model performance.

5) Data Visualization: Generated and validated model accuracy by creating a video of simulated pedestrian trajectories obtained from three models using OpenCV library.

## Results:
1) Entropy scores:
  (i) Steering Model: **4.46**
  (ii) Social Force Model: **5.06**
  (iii) Predictive Planning Model: **5.96**

2) Optimized the simulation for real-time applications, providing insights into crowd dynamics & potential safety issues.
