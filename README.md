# Plant-Detection

Agriculture is a field where automation isn’t given a significant importance.
During the course of this project, we made an attempt to scale down human labour by creating
an automaton which is able to indicate leaf health. Essentially the aim of this project is creating
a farming automaton which is able to work on line following principle which indicates the leaf
health by observing it. Here the complete project is done using MATLAB.
MATLAB is a proprietary multi-paradigm programming language and numerical
computing environment developed by MathWorks. MATLAB allows matrix
manipulations, plotting of functions and data, implementation of algorithms, creation
of user interfaces, and interfacing with programs written in other languages.
Our project indicates whether the identified leaf is of good health or bad health. This
project also looks forward to make a completely automated agricultural system in order
to make farming easier and more efficient.


# Image Classification using Feature-Based Matching in MATLAB

## Overview

This project is focused on building an image classification system using feature extraction and comparison in MATLAB. The system identifies and classifies test images based on their similarity to a set of trained images stored in a local database (`db.mat` file). The process involves three key stages: **Training**, **Classification**, and **Identification**.

---

## Project Structure

### 1. Code for Classification 
- The user selects a test image.
- Image features are extracted using a custom function (`FeatureStatistical`).
- Features of the test image are compared with stored training features from `db.mat`.
- The class with the minimum distance is selected as the detected class.
- Output is shown using a message box displaying the detected class.

### 2. Code for Training 
- The user selects an image and inputs the corresponding class label.
- Features are extracted from the image.
- The extracted features and class label are stored in the training database (`db.mat`).
- The database is saved and updated incrementally with each new training sample.

### 3. Code for Identification 
- Similar to classification, this module uses the trained database to identify a test image.
- It finds the closest match from the database and outputs the predicted class.

---

## How to Use

1. **Launch MATLAB**.
2. Place all `.m` files and the database file (`db.mat`) in the same working directory.
3. Run the training script to input and label images.
4. Use the classification script to test an unknown image.
5. Identification script can be used for verifying image recognition from trained data.

---

## Dependencies

- MATLAB R2018 or later
- Image Processing Toolbox (for `uigetfile`, `imread`, `imshow`, etc.)


## License

This project is developed for academic purposes and is open for modification and improvement.
