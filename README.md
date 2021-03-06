# Finding Lane Lines on the Road

The goals / steps of this project are the following:

Make a pipeline that finds lane lines on the road Reflect on your work in a written report

## Reflection

Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My Pipeline for identifying the lane lines consists of 6 steps. 
[x] First, I've converted the image to gray-scale for normalizing colours.
[x] Second, applied Gaussian smoothing to the image to improve the efficiency during Canny Edge Detection (Although it is a part in Canny's algorithm) 
[x] Third, Identified the edges (by pixel intensity variation) via setting up low and high threshold as 90 and 150. 
[x] Fourth, derived the vertices to arrive at the interested region 
[x] Fifth, Performed hough transformation with rho as 2, theta as pi/180, threshold as 50, minimum line length as 40 & maximum line gap as 150 
[x] Sixth, Overlay the transformed image to the original image to highlight the lane lines

Validated the pipeline against the test images & created corresponding output images under test images output

Validated the pipeline against the videos provided, created corresponding output of the video under test videos output

I've fine tuned parameters like Gaussian Kernel Size, Rho, Hough threshold to improve the accuracy of the solid line over the target.
