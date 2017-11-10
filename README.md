# Vision_Intelligence_and_Machine_Learning
Discover computer vision programming applications of image analysis, one of the most innovative fields of artificial intelligence.

![Demo][https://media.giphy.com/media/l4Epcsi3QwdQ2zyrC/giphy.gif]

Color Selection:
----
Applied color selection to the original RGB images, HSV images, and HSL images, and found out that using HSL will be the best color space to use.


Canny Edge Detection
----
The Canny edge detector is an edge detection operator that uses a multi-stage algorithm to detect a wide range of edges in images.
The Canny algorithm involves the following steps:
- Gray scaling the images: The Canny edge detection algorithm measures the intensity gradients of each pixel. So, we need to convert the images into gray scale in order to detect edges.
- Gaussian smoothing: Since all edge detection results are easily affected by image noise, it is essential to filter out the noise to prevent false detection caused by noise. To smooth the image, a Gaussian filter is applied to convolve with the image. This step will slightly smooth the image to reduce the effects of obvious noise on the edge detector.
- Find the intensity gradients of the image.
- Apply non-maximum suppression to get rid of spurious response to edge detection.
- Apply double threshold to determine potential edges.
- Track edge by hysteresis: Finalize the detection of edges by suppressing all the other edges that are weak and not connected to strong edges.
If an edge pixel’s gradient value is higher than the high threshold value, it is marked as a strong edge pixel. If an edge pixel’s gradient value is smaller than the high threshold value and larger than the low threshold value, it is marked as a weak edge pixel. If an edge pixel's value is smaller than the low threshold value, it will be suppressed. The two threshold values are empirically determined and their definition will depend on the content of a given input image.

Region of interest
---

Hough Transform
----
The Hough transform is a technique which can be used to isolate features of a particular shape within an image.

