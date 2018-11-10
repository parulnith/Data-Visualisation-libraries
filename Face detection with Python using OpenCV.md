# Face detection with Python using OpenCV

This tutorial will introduce you to the concept of computer vision in Python using OpenCV library and how you can utilise it to perform tasks like Facial detection.

## Introduction
Face detection is computer vision technology that helps to locate/visualise human faces in digital images. This technique is a specific use case of [object detection technology](https://en.wikipedia.org/wiki/Object_detection) that deals with detecting instances of semantic objects of a certain class (such as humans, buildings, or cars) in digital images and videos. With the advent of technology, face detection technology has gained a lot of importance in fields like photography, security and marketing. 

## Prerequisites

*This guide is mainly focused on OpenCV 3.x version**  (although most of the tutorials will work with OpenCV 2.x also). A prior knowledge on Python and Numpy is required before starting because they won’t be covered in this guide.  *Especially, a good knowledge on Numpy is must to write optimized codes in OpenCV-Python*.*

## Table of Contents

 1.   #### [OpenCV-Python](#introduction-to-r)
 -  1.Overview
 -   2.Installation

 2.   #### [Images as Numpy arrays](#getting-started)
 - Overview
 - Representing grayscale images as arrays
 - Representing coloured images as arrays
 - Numpy operations on images
 4. #### Images and OpenCV
 5. #### Object Detection
 6. #### Conclusion
 
 

# OpenCV-Python

## Overview

OpenCV was started at Intel in the year 1999 by **Gary Bradsky** . The first release came a little later in the year 2000.  OpenCV essentially  tands for **Open Source Computer Vision Library**. Although it is written in optimized C/C++, it has interfaces for both Python and Java along with C++. OpenCV boasts of a strong user base all over the world with its use increasing day by day due to surge in computer vision applications.

OpenCV-Python is the python API for OpenCV. You can think of it as a python wrapper around the C++ implementation of OpenCV. OpenCV-Python is not only fast (since the background consists of code written in C/C++) but is also easy to code and deploy(due to the Python wrapper in foreground). This makes it a great choice to perform computationally intensive programs.

Make sure that you have the following packages installed and running before installing OpenCV.
1.[Python](https://www.python.org/)
2. Numpy
3. Matplotlib


## Installation
OpenCV-Python supports all the leading platforms like Mac OS, Linux and Windows. In this article, I will briefly go over the steps required to install OpenCV in Windows and Mac.



# Images as Numpy arrays
An image is nothing but a standard Numpy array containing pixels of data points. More the number of pixels in an image, the better is its resolution. You can think of pixels to be tiny blocks of information arranged in form a 2 Dimensional grid and the depth of a pixel refers to the colour information present in it. 

Inorder to be  processed by a computer, an image needs to be converted into binary form. Check out the example below for more details:
![](https://github.com/parulnith/Face-Detection-in-Python-using-OpenCV/blob/master/Images%20as%20arrays.png)

Similarly, if we were to use more bits/pixels we would get more possible colours in the images.

    Number of colours/ shades = 2^bpp where bpp represents bits per pixel.

![enter image description here](https://github.com/parulnith/Face-Detection-in-Python-using-OpenCV/blob/master/Bits%20per%20pixels.png)

### Representation of a Grayscale image
A grayscale image consists og 8 bits per pixel. This means it can have 256 different shades where 0 pixel will represent black colour while 255 denotes white. For example the image below shows a grayscale image represented in the form of an array .

![enter image description here](https://github.com/parulnith/Face-Detection-in-Python-using-OpenCV/blob/master/graysclale.png)


### Representation of a Coloured image

Coloured images are represented as a combination of Red, Blue and Green colour and all other colours can be achieved by mixing these primary colours in correct proportions.
![enter image description here](https://github.com/parulnith/Face-Detection-in-Python-using-OpenCV/blob/master/Primary%20Colours.png)
[source](https://www.howtosmile.org/resource/smile-000-000-002-723) 
