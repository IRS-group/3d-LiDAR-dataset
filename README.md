# LiDAR Sensor Dataset

This repository contains datasets acquired using three different LiDAR sensors, mounted on a robotic mobile platform. The data is collected in various environments to facilitate comparison of the sensors' performance in 3D SLAM applications. This README provides an overview of the data acquisition setup, the environments, and instructions for using the dataset.

## Dataset Overview

The dataset includes LiDAR point cloud data acquired using the following sensors:

- **Velodyne Puck** (mounted at the bottom)
- **Ouster OS1** (mounted in the middle)
- **Livox Mid-360** (mounted at the top)

The sensors were vertically stacked on a Clearpath Robotics Jackal robot, ensuring minimal occlusion of the field of view (FOV) and enabling direct comparison of sensor data captured from the same trajectory.

The dataset consists of data captured in three different environments:

1. **Outdoor Garden**: A small garden containing trees, benches, lampposts, and surrounding buildings.
2. **Road Segment**: A section of road with construction signs, vehicles, and nearby buildings.
3. **Indoor Office Space**: An office environment with narrow corridors, desks, and large windows.

## Data Acquisition Setup

The sensors were mounted vertically on the Jackal robot to ensure consistent trajectory and environmental conditions for data collection. A two-meter proximity filter was applied to remove small-distance measurements and reduce variations between sensors for nearby objects.

- **Power**: All sensors were powered using the Jackal’s 12V power supply.
- **Data Transmission**: Sensors were connected to a TP-Link Archer MR600 router via LAN, and an external laptop was used to access the sensors and acquire data.
- **Control and Data Capture**: The **ROS (Robot Operating System)** framework was used to control the robot and manage data acquisition.

The setup allowed the robot to be teleoperated in various environments to collect comprehensive datasets for comparison between the three sensors.

## Tools and Processing

- **CloudCompare**: Used for point cloud visualization and sensor data comparison.
- **3D SLAM**: The collected data can be used for 3D SLAM experiments, with the same SLAM parameters applied across all sensors.

## Usage

To use this dataset, download the relevant environment datasets from the provided links. You can visualize the data using CloudCompare or any other point cloud processing software. The dataset is suitable for:

- Comparing sensor performance in 3D mapping.
- Benchmarking SLAM algorithms using different LiDAR sensor data.
- Point cloud processing experiments.

## Environments

The dataset contains point clouds for the following environments:

1. **Outdoor Garden**: 
   - Trees, benches, lampposts, surrounding buildings.
   - Best suited for outdoor SLAM or object detection tasks.
   
2. **Road Segment**: 
   - Road with construction signs, vehicles, and surrounding buildings.
   - Suitable for urban navigation and obstacle detection comparisons.
   
3. **Indoor Office Space**: 
   - Narrow corridors, desks, large windows.
   - Ideal for indoor navigation and mapping experiments.

## Dataset Links

The datasets are publicly available for download:

- [Download Dataset](https://ulisboa-my.sharepoint.com/:f:/g/personal/ist181272_tecnico_ulisboa_pt/ElBsT6U2FydElryo7fxur94BgxCxNkYMpErUhsex16xmSw?e=PBsuiW).

## How to Cite

If you use this dataset in your research, please cite the following paper:

> [Include citation to the relevant paper here when available]

---

For any questions or contributions, please feel free to submit an issue or a pull request.
