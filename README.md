[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

# CarND-Finding-Lane-Lines
This project takes images from a video feed then identifies the two nearest lanes.  The lanes are identified through image processing techniques.  The output is a video that displays these lines as overlays.

## Contents
1. Setup Instructions
2. Examples
3. Test_Images
4. Test_Videos
5. P1 Jupyter Notebook
6. Writeup
7. Test_Images_Output
8. Test_Videos_Output

## Code Sequence
1. Extract Image from Video

### Image Process - Pipeline
1. Grayscale Conversion
2. Gaussian Smoothing
3. Canny Filter
4. Region Masking
5. Hough Filter

### Draw Lines
1. Find Slope
2. Separate Left and Right Values
3. Generate Linear Fit
4. Extend end points to Region
5. Filter X and Y values outside image
6. Generate Line Overlay

## Shortcomings/Limitations
1. Lines must be linear
2. Obstructions may compromise performance
3. Color saturation can cause algorithm to fail

## Future Improvements
1. Region mask earlier in program to reduce processing time
