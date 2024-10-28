# Video Motion Estimation, Sentiment Analysis, and Gender Identification

## Overview
This repository contains three distinct tasks focused on video processing, sentiment analysis, and gender identification using traditional image processing techniques. Each task employs classical methods without relying on machine learning models, highlighting practical approaches to computer vision problems.

## Table of Contents
- [Task 1: Motion Estimation and Event Detection in a Video](#task-1-motion-estimation-and-event-detection-in-a-video)
- [Task 2: Estimating Sentiments of People in a Crowd – Gesture Analysis and Image Categorization](#task-2-estimating-sentiments-of-people-in-a-crowd--gesture-analysis-and-image-categorization)
- [Task 3: Gender Identification from Facial Features](#task-3-gender-identification-from-facial-features)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Task 1: Motion Estimation and Event Detection in a Video

### Objective
Detect motion and specific events in a video using frame differencing or optical flow techniques.

### Task Description
1. **Load Video**: Load the provided video using OpenCV.
2. **Motion Estimation**:  - Use frame differencing (histogram comparison) to detect changes between consecutive frames. 
   - Subtract consecutive frames and threshold the difference to identify regions of motion.
3. **Event Detection**:
   - Detect significant motion events, such as sudden movements or object appearances, based on motion intensity.
   - Identify and mark frames where events occur.
4. **Result**: 
   - Visualize motion by highlighting moving regions in each frame.
   - Annotate frames where events were detected, along with timestamps.

## Task 2: Estimating Sentiments of People in a Crowd – Gesture Analysis and Image Categorization

### Objective
Estimate the sentiments of individuals in a crowd using basic gesture analysis techniques.

### Task Description
1. **Load Image Set**: Load the provided images of people in a crowd.
2. **Preprocessing**: 
   - Use traditional face detection techniques to detect faces in the images.
   - Detect hand gestures based on skin color thresholding or simple shape analysis.
3. **Gesture Analysis**:
   - Perform facial feature extraction using geometric methods.
   - Classify basic emotions (happy, sad, neutral) based on facial geometry.
4. **Image Categorization**: - Categorize images based on the overall sentiment detected by averaging individual sentiments.
5. **Result**: 
   - Output the sentiment of each individual and the overall sentiment of the crowd.
   - Display key facial features used for gesture analysis.

## Task 3: Gender Identification from Facial Features

### Objective
Identify the gender of individuals based on facial features using traditional image processing techniques.

### Task Description
1. **Load Dataset**: Load the facial image dataset labeled with gender.
   **Link** : https://www.kaggle.com/datasets/cashutosh/gender-classification-dataset
3. **Preprocessing**: 
   - Detect faces in the images using techniques like Haar Cascades.
   - Normalize and crop the facial regions for feature extraction.
4. **Feature Extraction**:
   - Extract facial features using geometric and texture-based methods.
5. **Rule-Based Gender Identification**: 
   - Use predefined rules based on facial geometry and texture to classify gender.
6. **Result**: 
   - Output the identified gender for each image.
   - Display extracted facial features and explanations for decisions made.

## Installation
To run these tasks, ensure you have the necessary dependencies installed. You can set up a Python virtual environment and install the required libraries with the following commands:

```bash
pip install opencv-python matplotlib
