# Face, License Plate, and Lane Detection - December 2023

📄 You can read the full project report here: [Presentation.pdf](Presentation.pdf)  

## Overview
This project, created for the Image Processing course final in December 2023 by Noora Noor and Christina Chum, focuses on implementing various image processing techniques, including Face Detection, License Plate Detection, and Lane Detection. The project is implemented in Python and utilizes Google Colab, OpenCV, and Matplotlib.

## Table of Contents
1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Lane Detection](#lane-detection)
4. [Enhancing or Making Image Better](#enhancing-or-making-image-better)
5. [Face Recognition](#face-recognition)
6. [Face Recognition Combined with Enhancing or Making Image Better](#face-recognition-combined-with-enhancing-or-making-image-better)
7. [Pedestrian Recognition](#pedestrian-recognition)
8. [License Plate Recognition](#license-plate-recognition)
9. [Conclusion](#conclusion)
10. [Additional Documentation](#additional-documentation)
11. [License](#license)
    

## Introduction
This project implements various image processing techniques to accomplish tasks such as lane detection, enhancing image quality, face recognition, pedestrian recognition, and license plate recognition.

## Setup
To run the project, follow these steps:
1. Clone or download the project repository.
2. Ensure Python is installed on your system.
3. Install required libraries using pip:
    ```
    pip install opencv-python-headless matplotlib
    ```
4. Open the project in Google Colab or any Python IDE.

## Lane Detection
- Probabilistic Hough Line is used to perform lane detection on a grayscale image.
- Canny edge detection highlights potential lane lines.
- Hough Transform identifies lines corresponding to lanes.
- Filtered lines recognized as lane lines based on orientation are drawn in red.

## Enhancing or Making Image Better
- Converts image from BGR to RGB.
- Adjusts contrast and brightness.
- Applies bilateral filter to reduce noise.
- Applies Gaussian blur to remove blur.
- Enhances contrast and brightness.

## Face Recognition
- Uses Haar Cascade for face detection.
- Draws rectangles around detected faces.
- Converts BGR to RGB for display.

## Face Recognition Combined with Enhancing or Making Image Better
- Haar Cascade used for face classification.
- Converts image from BGR to GRAY.
- Enhances photo by changing contrast and brightness.

## Pedestrian Recognition
- HOG descriptor used to detect persons.
- Draws rectangles around detected pedestrians.
- Applies Gaussian blur to blur out background.
- Zooms in on pedestrians.

## License Plate Recognition
- Converts image from BGR to GRAY.
- Applies Gaussian blur to reduce noise.
- Thresholding to create binary image.
- Contour threshold image.
- Masks the detected license plate.
- Calculates the coordinates for the plate.
- Crops the plate.

## Conclusion
This project demonstrates the practical application of image processing techniques for various tasks such as lane detection, enhancing image quality, face recognition, pedestrian recognition, and license plate recognition. It showcases the versatility and utility of computer vision algorithms in real-world applications.


## Additional Documentation
- [Project Report](Presentation.pdf): Detailed project report providing in-depth analysis, implementation details, and results.

## License
This project is licensed under the [MIT License](LICENSE).
