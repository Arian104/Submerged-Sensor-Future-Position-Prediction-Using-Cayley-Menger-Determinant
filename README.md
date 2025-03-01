# Submerged Sensor Future Position Prediction Using Cayley-Menger Determinant (CMD)

## Project Overview

This project focuses on predicting the future positions of submerged sensors using the **Cayley-Menger Determinant (CMD)** combined with machine learning models. By leveraging a **six-beacon setup**, we enable quick and reliable localization of submerged sensors, even in dynamic underwater environments. The system captures multiple readings simultaneously, reducing the time required for data collection and improving accuracy by averaging positions. This approach minimizes errors and allows for real-time tracking and prediction of sensor movements, such as drifting or sinking.

To predict future positions, we employ machine learning models, including **Linear Regression**, **Random Forest**, and **Recurrent Neural Networks (RNN)**. These models analyze historical sensor data to forecast future coordinates, providing valuable insights for applications like underwater navigation, search and rescue operations, and environmental monitoring.

---

## Key Features

- **Six-Beacon Configuration**: Enables simultaneous data collection, reducing localization time and improving accuracy.
- **Dynamic Environment Adaptation**: Capable of tracking moving or sinking sensors by combining multiple readings with machine learning predictions.
- **Machine Learning Integration**: Utilizes Linear Regression, Random Forest, and RNN models to predict future sensor positions.
- **Error Reduction**: Multiple readings and averaging techniques minimize localization errors.
- **Real-Time Tracking**: Provides real-time updates on sensor positions and future trajectories.

---

## Methodology

### Localization Using Cayley-Menger Determinant (CMD)
The **Cayley-Menger Determinant** is used to compute the geometric positions of submerged sensors based on pairwise distance measurements. This method provides a **closed-form solution**, making it computationally efficient and robust for underwater environments.

### Six-Beacon Setup
Our six-beacon configuration allows for:
- Simultaneous distance measurements, reducing data collection time.
- Averaging multiple readings to minimize errors.
- Real-time tracking of moving or sinking sensors.

### Machine Learning for Future Position Prediction
We employ the following machine learning models to predict future sensor positions:
1. **Linear Regression**:
   - MSE for S3_x: 1.550161407902013
   - MSE for S3_y: 3.9619723362917267
   - MAE for S3_x: 0.9978410563108646
   - MAE for S3_y: 1.5490609928485373
   - R² for S3_x: 0.98
   - R² for S3_y: 0.96
   - Accuracy: 93.63%

2. **Random Forest**:
   - MSE for S3_x: 2.0653192636925963
   - MSE for S3_y: 5.898981018874267
   - MAE for S3_x: 1.112221284962562
   - MAE for S3_y: 2.062574748344956
   - R² for S3_x: 0.97
   - R² for S3_y: 0.94
   - Accuracy: 90.92%

3. **Recurrent Neural Network (RNN)**:
   - MSE for S3_x: 3.7648746673226525
   - MSE for S3_y: 3.2694436419214714
   - R² for S3_x: 0.90
   - R² for S3_y: 0.94
   - Accuracy: 84.47%

---

## Results and Comparison

### Model Performance
- **Linear Regression** delivered the highest accuracy (93.63%) and the lowest errors, making it the most effective model for this task.
- **RNN** also performed well, particularly in predicting the y-coordinate (R² = 0.94).
- **Random Forest** provided a balance between accuracy and computational efficiency.

### Key Insights
- Linear Regression and RNN are the most suitable models for predicting submerged sensor positions.
- The six-beacon setup significantly improves localization accuracy and reduces errors.
- Real-time tracking and future position prediction are achievable with this system, even in dynamic underwater environments.

---

## Applications

This system has a wide range of applications, including:
- **Search and Rescue Operations**: Locating and tracking submerged objects or vehicles.
- **Environmental Monitoring**: Tracking underwater sensors for data collection.
- **Underwater Navigation**: Assisting autonomous underwater vehicles (AUVs) in navigation and positioning.
- **Marine Research**: Studying underwater phenomena and tracking marine life.

---

