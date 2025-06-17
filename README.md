# EGR 598: Pedestrian Detection with Sensor Fusion in CARLA

> My Master's capstone project developing a robust pedestrian detection system for autonomous vehicles by fusing LiDAR and Radar data in the high-fidelity CARLA simulator. This project showcases advanced skills in sensor fusion, machine learning, and simulation.

---

### 🎯 Project Objective

[cite_start]The primary goal was to overcome the limitations of single-sensor systems by developing a multi-modal fusion framework that enables precise and reliable detection of pedestrians in varied and adverse environmental conditions like rain, fog, and nighttime. 

---

### 🛠️ Methodology & Technology

* [cite_start]**Simulation Environment:** All testing and validation were performed in the **CARLA open-source simulator** to ensure repeatability and control over diverse weather and lighting conditions. 
* [cite_start]**Core Algorithm:** Implemented the **PointPillars** algorithm to efficiently process raw LiDAR point cloud data.  [cite_start]This converts the sparse point cloud into a compact pseudo-image representation, allowing for fast and effective 2D convolutional processing. 
* [cite_start]**Sensor Fusion:** Integrated **LiDAR** data (for high-resolution spatial information) with **Radar** data (for accurate velocity estimates) to create a more robust perception system. 
* [cite_start]**State Estimation:** Utilized a **Kalman Filter** to integrate the sensor data over time, providing optimal predictions of a pedestrian's position and velocity while mitigating sensor noise. 

---

### 📊 Key Results

The sensor fusion model demonstrated significant performance gains over a LiDAR-only baseline.

* [cite_start]**Detection Accuracy:** Improved from 78% (LiDAR only) to **85%** with fusion. 
* [cite_start]**Object Recall:** Increased dramatically from 75% to **90%**, meaning the system was much better at finding objects that the single sensor missed. 
* [cite_start]**Precision:** Rose from 80% to **92%**, indicating a significant reduction in false positive detections. 
* [cite_start]**Real-Time Performance:** Maintained an efficient **42 FPS** inference time, proving its suitability for real-world autonomous systems. 

<p align="center">
  <img src="URL_TO_YOUR_RESULTS_GRAPH_SCREENSHOT" alt="Performance Metrics Graph">
</p>

*(**Pro Tip:** Take a screenshot of the "Performance Metrics: LiDAR Only vs. LiDAR + Radar Fusion" bar chart from your report, upload it to this repository, and paste its link in the `src` above.)*

---

### 📄 View Full Project Files

* [**View the Final Report (PDF)**](./Aniket%20Mishra%20EGR598%20Final%20Report.pdf)
* [**View the Final Presentation (PDF)**](./EGR%20598%20Final%20Presentation%20Aniket%20Mishra.pdf)
