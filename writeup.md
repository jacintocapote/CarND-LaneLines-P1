# **Finding Lane Lines on the Road** 

## By Jacinto Capote Robles

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 6 steps:
* We use a crop of the picture (Based in the size of the image in another case we can get errors)
* We convert image to HLS is the best space color for detect lines and we creat to mask for white and yellow.
* Convert the image to grayscale
* Pass gausian filter and convert to canny
* Pass a hough filter.
* Add weight to lines based on slope to classificate between left and right.
![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


We move the position of the camera or we are over a road without lines.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to identify if we are into left or right road, work with raining, ...

