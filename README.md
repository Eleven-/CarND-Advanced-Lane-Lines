[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

# CarND-Finding-Lane-Lines
This project takes images from a video feed then identifies the two nearest lanes.  The lanes are identified through image processing techniques.  The output is a video that displays these lines as overlays.

![Output Lane Lines Image](examples/laneLines_thirdPass.jpg)

## Overview
The code extracts images from a video of the road taken from cameras mounted on a car.  These images are filtered for the lanes.

**Image Process - Pipeline**

1. Grayscale Conversion

2. Gaussian Smoothing - Reduce Noise

3. Canny Filter - Edge Detection

4. Region Masking - Pre-Process

5. Hough Filter - Line Segment Detection

## Motivation
The motivation behind this problem is to address one aspect of the self-driving car challenge.  Identifying lanes provides the autonomous software more information about its environment.  The software then can make a decision and adjust its controls to safely navigate.

## Installation

**Step 1:** Set up the [CarND Term1 Starter Kit](https://classroom.udacity.com/nanodegrees/nd013/parts/fbf77062-5703-404e-b60c-95b78b2f3f9e/modules/83ec35ee-1e02-48a5-bdb7-d244bd47c2dc/lessons/8c82408b-a217-4d09-b81d-1bda4c6380ef/concepts/4f1870e0-3849-43e4-b670-12e6f2d4b7a7) if you haven't already.

**Step 2:** Open [code](https://github.com/Eleven-/CarND-Finding-Lane-Lines/blob/master/P1.ipynb) in a Jupyter Notebook

Jupyter is an Ipython notebook where you can run blocks of code and see results interactively.  All the code for this project is contained in a Jupyter notebook. To start Jupyter in your browser, use terminal to navigate to your project directory and then run the following command at the terminal prompt (be sure you've activated your Python 3 carnd-term1 environment as described in the [CarND Term1 Starter Kit](https://github.com/udacity/CarND-Term1-Starter-Kit/blob/master/README.md) installation instructions!):

`> jupyter notebook`

A browser window will appear showing the contents of the current directory.  Click on the file called "P1.ipynb".  Another browser window will appear displaying the notebook.  Follow the instructions in the notebook to complete the project.  

## Tests
For testing there are test images, test videos, and examples for comparison purposes.

-[test images](https://github.com/Eleven-/CarND-Finding-Lane-Lines/tree/master/test_images)

-[test videos](https://github.com/Eleven-/CarND-Finding-Lane-Lines/tree/master/test_videos)

-[examples](https://github.com/Eleven-/CarND-Finding-Lane-Lines/tree/master/examples)

## Shortcomings/Limitations
1. Lines must be linear
2. Obstructions may compromise performance
3. Color saturation can cause algorithm to fail
4. Image size is hard coded so it may be incompatible with different perspectives/sizes

## Future Improvements
1. Region mask earlier in program to reduce processing time
