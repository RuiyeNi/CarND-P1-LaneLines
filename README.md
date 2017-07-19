Piplines and Reflection
---
## 1. Describe the pipeline
My pipeline included six steps. 

**Step1:** converted a color image into grayscale.

**Step2:** applied a gaussian kernel to smooth gray image.

**Step3:** detected edges with canny edge detection by pixel thresholding.

**Step4:** created a four side mask so that only edges in the area of the mask would be considered for further lane detection.

**Step5:** transformed the image from image space to hough space and identified lines with five parameters including distance resolution, aungular resolution, minimum number of votes, mininum number of pixels, and maximm gap in pixels. 

**Step6:** drawed identified left and right side lines of the lane on the color image.


## 2. Identify any shortcomings
I applied a simple method to draw solid lines by figuring out the the maximum and minimum of the abscissa and the ordinate values and drawed lines defined by point (Xmin, Ymax) and point (Xmax, Ymin), left and right lines were distinguished by slope. This method has one shortcoming that when a to-be detected segmented line in a image started from somewhere far from the bottom of a image, the finally drawed line could not cover the bottom area of the image. Another shortcoming is that in the challenge video, drawed lines were not as stable as in the first two video, espeically the right side segmented line jumped a lot.

## 3. Suggest possible improvements
One of the possible improvements for the first shortcoming is to extrapolate a line defined by point (Xmin, Ymax) and point (Xman, Ymin) so that a line could be drawed from the bottom of a image. Another improvement could be made is to define a more delicate mask so that shades and other marks on the road would not affect the edges detection.
