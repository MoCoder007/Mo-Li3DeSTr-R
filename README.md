
# Introduction

Autonomous vehicles (AVs) rely heavily on LiDAR (Light Detection and Ranging) for precise 3D object detection. However, LiDAR's performance can significantly degrade in rainy conditions, affecting the safety and efficiency of AVs. Mo-Li3DeSTr addresses this challenge by introducing an innovative architecture that enhances the interpretability of noisy data, enabling reliable navigation in diverse weather scenarios.

# Mo-Li3DeSTr: Robust LiDAR Sensor for 3D Object Detection in Rainy Weather

Mo-Li3DeSTr is a cutting-edge research project focused on enhancing 3D object detection capabilities of LiDAR sensors under adverse weather conditions, specifically during rain. Developed by Mohamed Elatfi, Haigen Min, Akram Al-Radaei, and Anass Taoussi at the School of Information Engineering, Chang’an University, China, this project presents a transformative model that integrates transformer networks with LiDAR technology to improve detection robustness.

The Mo-Li3DeSTr project, developed at Chang’an University, represents a significant advancement in the field of autonomous vehicle (AV) technologies, especially in enhancing LiDAR sensors' effectiveness under challenging weather conditions such as rain. This integration of transformer networks with LiDAR technology not only improves the robustness of detection systems but also enhances their interpretability when dealing with noisy, rain-distorted data. Below, I detail the two models developed under this project: Mo-Li3DeSTr-C and Mo-Li3DeSTr-R, focusing on their training environments, datasets, and performance metrics.

## Mo-Li3DeSTr-C Model

Training and Testing Environment:
- *Dataset Used for Training: KITTI dataset
- *Simulation Environment for Testing: CARLA simulation

### Key Characteristics:

- *Purpose: Tailored to bridge the gap between traditional datasets and realistic, dynamic conditions that AVs face in real-world scenarios.
- *Technology Integration: Utilizes a transformer-based architecture specifically adapted for processing the 3D point clouds generated by LiDAR sensors in vehicles.
- *Advantages: Enhances data interpretability under adverse weather by effectively filtering out the noise introduced by rain in the sensor inputs.

### Performance Metrics:

- *Average Precision (AP) Scores: Demonstrates superior AP scores, particularly in scenarios with various degrees of detection difficulty caused by rainy conditions.
- *Benchmark Comparison: Outperforms standard benchmarks that typically do not perform well under adverse weather conditions.

## Mo-Li3DeSTr-R Model

Training and Testing Conditions:
- *Dataset Used for Both Training and Testing: SHIFT dataset

### Key Characteristics:

- *Purpose: Developed to specifically address and test the capabilities of AV technologies in rain-affected environments using a more challenging and varied dataset.
- *Technology Integration: Incorporates advanced transformer techniques to process complex datasets like SHIFT, which are designed to simulate severe weather conditions more accurately.
- *Adaptation and Robustness: Focuses on robustness against the high variability and unpredictability of environmental conditions depicted in the SHIFT dataset.

### Performance Metrics:

- *Average Precision (AP) Scores: Expected to provide high AP values across different levels of rain intensity, validating the model’s effectiveness in noisy, high-disturbance environments.
- *Real-World Applicability: Tests conducted using the SHIFT dataset offer insights into the practical challenges and performance expectations in real-life AV navigation during adverse weather.

## Overall Impact and Innovations

The Mo-Li3DeSTr project showcases critical innovations:
- *Integration of Transformers with LiDAR Technology: This hybrid approach leverages the spatial processing strengths of transformer networks to enhance the interpretability of 3D point clouds in noisy conditions like heavy rain.
- *Enhanced Noise Interpretation Capabilities: By improving how sensors interpret distorted data, these models help maintain reliable detection and navigation systems in AVs, even during unfavorable weather conditions.
- *Setting New Benchmarks: With their high AP scores and robust performance under rain, these models set new standards for AV sensory technologies, particularly in terms of reliability and effectiveness in diverse weather scenarios.

## Technologies Used

- *Python* for core development.
- *PyTorch* as the primary deep learning framework.
- The *KITTI dataset* for training
- Carla Simulation for testing Mo-Li3DeSTr-C Model
- *SHIFT dataset* for training and testing 
- Advanced *transformer network models* for data processing and interpretation.

## Future Directions

- *Further Development: Ongoing improvements will focus on optimizing these models for other adverse conditions such as fog and snow.
- *Cross-Dataset Efficiency: Future versions could explore hybrid training regimes that use multiple datasets to enhance generalizability and reliability across various environmental scenarios.
- *Real-Time Processing Enhancements: Efforts to reduce the computational demands of transformer networks to facilitate real-time processing capabilities in AVs.


## MODEL ARCHITECTURE (MO-Li3DeSTr)
![MODEL ARCHITECTURE (MO-Li3DeSTr)](https://github.com/MoCoder007/Mo-Li3DeSTr--Robust-LiDAR-Sensor-for-3D-Object-Detection-with-Transformers-Network-in-Rainy-Weather/blob/main/Model%20Architecture.PNG))

##  A qualitative Comparison in different Situations
![A qualitative Comparison in different Situations](https://github.com/MoCoder007/Mo-Li3DeSTr--Robust-LiDAR-Sensor-for-3D-Object-Detection-with-Transformers-Network-in-Rainy-Weather-/blob/main/Agualitative%20Comparison%20in%20different%20situations.png)

## Mo-Li3DeSTr detection in light Rain
![Mo-Li3DeSTr detection in light Rain](https://github.com/MoCoder007/Mo-Li3DeSTr--Robust-LiDAR-Sensor-for-3D-Object-Detection-with-Transformers-Network-in-Rainy-Weather-/blob/main/Mo-Li3DeSTr%20detection%20rain%20rate%20(Light%20Rain).jpeg)

## Mo-Li3DeSTr detection in Heavy Rain
![Mo-Li3DeSTr detection in Heavy Rain](https://github.com/MoCoder007/Mo-Li3DeSTr--Robust-LiDAR-Sensor-for-3D-Object-Detection-with-Transformers-Network-in-Rainy-Weather-/blob/main/Mo-Li3DeSTr%20detection%20rain%20rate%20(Heavy%20Rain).jpeg)
