# SIFT-BuitIn_VS_Custom_Implementation-

This repository demonstrates the implementation and comparison of built-in and custom implementations of the Scale-Invariant Feature Transform (SIFT), a popular feature detection and description algorithm widely used in computer vision tasks such as object recognition, image stitching, and motion tracking.

## Introduction
SIFT is a robust algorithm for detecting and describing local features in images. It is scale and rotation-invariant, making it a cornerstone for many computer vision applications. This project includes:

- Usage of OpenCV’s built-in SIFT implementation.
- A custom implementation of SIFT, showcasing a deeper understanding of its core components and flexibility for modifications.

## Features
- Detects keypoints in an image that are invariant to scale and rotation.
- Extracts feature descriptors from keypoints.
- Visualizes keypoints and matches between images.
- Comparison of performance and results between built-in and custom implementations.

## Implementation Details
### Built-in SIFT
Utilizes OpenCV's built-in SIFT functionality:

- Fast and optimized for large-scale applications.
- Easy to use with OpenCV's cv2.SIFT_create() method.
- Visualizations for detected keypoints and descriptor matches.

### Custom SIFT
A step-by-step implementation of SIFT:

- Gaussian Blur Pyramid: Constructing image pyramids with varying levels of blur.
- Difference of Gaussians (DoG): Calculating the difference between successive layers in the pyramid to identify potential keypoints.
- Keypoint Localization: Refining detected keypoints using thresholds for stability.
- Orientation Assignment: Assigning a dominant orientation to each keypoint for rotation invariance.
- Descriptor Generation: Generating feature descriptors by creating histograms of local gradients around each keypoint.

## Results
### Built-in SIFT:
- Faster execution.
- Highly accurate keypoint detection and matching.
### Custom SIFT:
- Provides flexibility and deeper insight into the algorithm.
- Slightly slower and may require parameter tuning for optimal results.
- Sample visualizations for both implementations are included in the repository under the results folder.

## Future Work
- Extend the custom implementation to include GPU acceleration for faster processing.
- Experiment with SIFT-based applications like image stitching and object tracking.
- Add comparisons with other feature detection algorithms like ORB and SURF

