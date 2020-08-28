# Course Introduction and Setup

**Topics we will learn:** OpenCV, Computer vision: Object detection, Photo restoration, object tracking, and many more.

**Prerequisites:** Basic knowledge of python.

**Requirments:** Basic programming, High school level maths, A webcam, Python, OpenCV

>We will be building 12 mini-projects during this course.


**Computer vision:** It is a cutting edge field of computer science that aims to enable computers to understand what is being seen in an image.

**Challenge in computer vision:** Low light, the orientation of objects, Illusions, image quality, etc.

**Why python?**
*  Easiest language for beginners.
*  Extremely powerful for data science and ML.
*  Stores images in bumpy arrays, so the process is quick.

**OpenCV**: Open-source library for computer vision.

To install use: `pip install opencv`

>Using anaconda will be a better option.

# Basics of Computer Vision and OpenCV

**What are images?**

* 2-D representation of the spectrum of light.
* Image consists of small pixels, where each pixel corresponds to a particular color i.e it has a certain RGB value.

> In OpenCV we follow BGR format.

**How computer store images?**
* In pixel RGB form. Each ranging from 0 to 255, where 255 is white.
* In computers they are stored in 3-dimensional arrays, here x and y varies, but at a z-axis, we have 3 stacks, each for RGB.
* For B/W images, stored in 2-d arrays, where one pixel can have just two values, 0 and 1.
* For grayscale images, it is same as B/W except there is a range of 0 to 255 instead of just 0 and 1.


**OpenCV**

* Open Source Computer Vision, an intel initiative.
* Written in C++
* Visit opencv.org for documentation and learning more.

Import using `import cv2`

Use `cv2.imread('path')` to read image.

Use `cv2.imshow()` to view.

`image.shape` for dimensions.

**Grayscaling**

*  It is a process of converting RGB images in grayscale or shades of gray.

*  It is important part in any model, as it makes process faster.

>Read image, then `x=cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)` and x is your grayscale image.


**Color Spaces**

It is a way to represent colors, like RGB, HSV and CMYK. 

* **RGB** consists of Red, Gree and blue mixed differently at different pixels.

* **HSV** is Hue, saturation and Value/Brightness. (most usefull)
   *  **Hue:**  Color value (0-179)
   *  **Saturation:**  Vibrancy of color (0-255)
   *  **Value:**  Brightness (0-255)
   
**Histogram representation of images**

`histogram=cv2.calcHist((image),[0], None, [256], [0,256])`

Here, image is read image, [0] is the number of channels, None is for Mask, [256] is histogram size, and [0,256] is range.

Then use matplotlib to show the histogram.

**Drawing on Images**

**Line:** `cv2.line(image, (0,0), (511,511), (127,127,0), 5)` here parameters are: image, then starting point, then ending point, color of lin and then thickness of line.

**Rectangle:** `cv2.rectangle(image, (100,00), (300,250), (127,127,0), 5)` here parameters are: same as line.

**Circle:** `cv2.rectangle(image, (100,10), 100, (127,127,0), 5)` here everything same except 2nd one is center, and third is radius.

>These are important parts as shapes are used in any application to show sections, detected objects, or represent any area after processing.


# Image Manipulations - The Many Ways You Can Change Images


**Transformations, Affine and Non-Affine**

| Affine | Non-Affine |
| ------ | ------ |
| Scaling, Rotation and Translation | Projective transform or Homography |
| Preserves parallelism, length, and angle. |Do not preserves parallelism, length, and angle, but preserves collinearity and incidence is maintained. | 
|Square will be a square, just change in size or rotation.| Square can become a rhombus or rectangle or parallelogram.|
