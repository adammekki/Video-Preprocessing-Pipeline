# 🚗 Video Preprocessing & Lane Detection for Autonomous Driving

This project implements a **video preprocessing pipeline** using classical computer vision techniques to enhance dashcam footage and highlight road lanes. It explores fundamental image processing methods that serve as building blocks for autonomous driving systems, prior to applying deep learning models.

---

## 📹 Project Overview

The pipeline processes raw driving footage by:
1. **Extracting frames** from video.
2. **Preprocessing images** through grayscale conversion, histogram analysis, histogram equalization, Fourier transforms, edge detection, and kernel filtering.
3. **Highlighting road lanes** with edge detection, dilation, and overlay techniques.
4. **Experimenting with Hough Transform and contour detection** to detect lane lines and objects.

---

## 🔍 Implemented Techniques

- **Frame Extraction**  
  Converted videos into individual frames for analysis.

- **Histogram Analysis & Equalization**  
  Improved contrast in low-visibility conditions (e.g., night driving, tunnels).

- **Fourier Transform**  
  Analyzed frequency components of frames to filter noise and detect road textures.

- **Edge Detection**  
  Applied Canny edge detection to identify lane markings, road boundaries, and object outlines.

- **Kernel Filtering**  
  Used Gaussian blur and median filtering to reduce noise and enhance key features.

- **Lane Highlighting**  
  Combined grayscale conversion, Gaussian blur, edge detection, and dilation to overlay detected lane areas in green on video frames.

- **Bonus: Line & Object Detection**  
  - **Hough Transform** for detecting lane-like lines.  
  - **Contour Detection** for bounding potential obstacles.

---

## 📊 Results

- Processed video outputs with highlighted lanes were saved as new `.mp4` files.  
- Preprocessing techniques demonstrated improved visibility of structural features, critical for downstream tasks in autonomous driving.  
- Classical CV methods proved effective on limited resources, showing their value in embedded or real-time systems.

*(Sample before/after frames or short video clips can be added here to showcase results.)*

---

## 🛠️ Tech Stack

- **Python**
- **OpenCV** (image & video processing)
- **NumPy** (Fourier transforms, array manipulation)
- **Matplotlib** (visualizations)

---

## 📂 Repository Structure

- Preprocessing Pipeline.ipynb # Full pipeline code
- video.mp4 # Sample input video
- highlighted_lanes.mp4 # Processed output with lane overlay
- README.md # Project documentation

---

## 🎯 Key Learnings

- Hands-on implementation of classical image processing techniques.  
- Practical application of **histogram analysis, Fourier transforms, and edge detection** in real driving contexts.  
- Understanding how preprocessing enhances data quality for autonomous driving models.  
- Experience with **video I/O, frame-level transformations, and feature extraction**.

---

## 📌 Next Steps

- Integrate advanced methods such as **deep learning-based lane segmentation (U-Net, DeepLab)**.  
- Fuse results with **sensor data (LiDAR, radar)** for multimodal perception.  
- Optimize pipeline for **real-time deployment on embedded systems**.

---

## 👤 Author

Developed by **Adam Mekki**  
As part of an academic project on image preprocessing for autonomous driving.
