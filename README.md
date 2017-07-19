Piplines and Reflection
---
## 1. Describe the pipeline
My pipeline included six steps. 

Step1: converted a color image into grayscale.

Step2: applied a gaussian kernel to smooth gray image.

Step3: detected edges with canny edge detection by pixel thresholding.

Step4: created a four side mask so that only edges in the area of the mask would be considered for further lane detection.

Step5: transform image from image space to hough space and identified lines with five parameters including distance resolution, aungular resolution, minimum number of votes, mininum number of pixels, and maximm gap in pixels. 

Step6: drawed identified left and right side lines of the lane.

a gaussian kernel was applied to smooth the grayscalor image. In the third step, canny edge detected was used to 

## 2. Identify any shortcomings

## 3. Suggest possible improvements
