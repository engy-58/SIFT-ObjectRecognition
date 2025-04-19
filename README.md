# SIFT-ObjectRecognition
A mini project for detecting and tracking objects in images and video using the SIFT algorithm in OpenCV

# Object Detection with SIFT in OpenCV

This repository contains two Jupyter Notebooks that demonstrate how to use the Scale-Invariant Feature Transform (SIFT) algorithm for object detection in images and videos using OpenCV.

## Table of Contents

- [Introduction](#introduction)
- [Image Object Detection](#image-object-detection)
- [Video Object Detection](#video-object-detection)
- [Requirements](#requirements)
- [Usage](#usage)
- [License](#license)

## Introduction

SIFT is a powerful feature detection algorithm that is invariant to scale, rotation, and illumination changes. It is widely used in computer vision tasks for detecting and matching keypoints between images.

## Image Object Detection

### Overview

The image object detection notebook demonstrates how to detect and locate an object within a target image using a query image. The process involves:

1. **Uploading Images:** Users upload a query image (the object to find) and a target image (where to find the object).
2. **Feature Detection:** SIFT is used to detect keypoints and descriptors in both images.
3. **Feature Matching:** A FLANN-based matcher is used to find good matches between the query and target images.
4. **Homography and Bounding Box:** If enough matches are found, a homography is computed to locate the object in the target image, and a bounding box is drawn around it.

### Key Features

- **Robust Matching:** Uses a ratio test to filter out poor matches.
- **Homography Estimation:** Computes a homography to accurately locate the object.
- **Visualization:** Displays the query and target images with detected matches and bounding boxes.

## Video Object Detection

### Overview

The video object detection notebook extends the image detection capabilities to video. It tracks an object throughout a video using the following steps:

1. **Uploading Files:** Users upload a query image and a video file.
2. **Feature Detection and Matching:** SIFT is used to detect and match features frame by frame.
3. **Object Tracking:** The object is tracked across frames using homography and keypoint matching.
4. **Output Video:** The processed video with annotations is saved and can be downloaded.

### Key Features

- **Frame-by-Frame Processing:** Efficiently processes video frames to detect and track objects.
- **Real-Time Feedback:** Provides progress updates and sample frames during processing.
- **Output Video:** Saves the annotated video for offline review.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- Matplotlib
- Google Colab (for file uploads and processing)

## Usage

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/engy-58/SIFT-ObjectRecognition
   cd SIFT-ObjectRecognition
   ```

2. **Open the Notebooks:**
   - Use Jupyter Notebook or Google Colab to open and run the notebooks.

3. **Follow the Instructions:**
   - Each notebook contains step-by-step instructions and explanations to guide you through the process.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
