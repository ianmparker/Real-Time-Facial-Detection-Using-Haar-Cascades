# Real-Time-Facial-Detection-Using-Haar-Cascades

My LinkedIn: https://www.linkedin.com/in/ian-parker-596011142/

![realtime_facial_detection](https://github.com/ianmparker/Real-Time-Facial-Detection-Using-Haar-Cascade/assets/18231849/00fa3c4b-b403-425a-b580-bb0c43c3f77d)


-----------------------------------------------

## Introduction

In this repository you will find a C++ project that showcases the uses of Haar Cascades for object detection. 

-----------------------------------------------

## What is a Haar Cascade? 

![image](https://github.com/ianmparker/Real-Time-Facial-Detection-Using-Haar-Cascade/assets/18231849/95110121-c636-4ed7-b4b3-09f30065c16d)

Haar Cascades are machine learning object detection algorithms. 

They use Haar features to determine the likelihood of a certain point being part of an object. 

In this case that object is a human face.

Haar Cascades make use of a kind of filter to perform feature extraction from the given image. 

These filters inspect only one portion of the image at a time. 

The intensity of the pixels in the white portion and in the black portion is added. 

The result of subtraction of these two summations is the feature extracted value. 

Haar cascade combines multiple Haar features in a hierarchy to build a classifier.

Instead of analyzing the entire image with each Haar feature, cascades break down the detection process into stages, each consisting of a set of features.

----------------------------------------------
## Installation

If you are new to Coding, C++, or IDE's like Visual Studios, you might find this tutorial to help you set up your environment.  
  - https://github.com/murtazahassan/Learn-OpenCV-cpp-in-4-Hours/blob/main/Opecv%20Windows%20Installation.md

----------------------------------------------
## Using an Image instead of a Webcam
![image](https://github.com/ianmparker/Real-Time-Facial-Detection-Using-Haar-Cascade/assets/18231849/8959d37c-b4b6-4835-b09f-57e41c8b827d)

You may notice a large chunk of commented out code at the bottom of FacialDetection.cpp.

This is a a bonus section for detecting faces from images instead of using a webcam's live stream. 

You can edit the path to that of your own photo to try this with your own still image. 


---------------------------------------------
## Improvements/Next Steps 
![Smooches from beanie](https://github.com/ianmparker/Real-Time-Facial-Detection-Using-Haar-Cascade/assets/18231849/295193fd-0484-41b0-90ba-6bcfab7607c9)

As it currently stands the system has a hard time detecting faces while moving or when making certain expressions. 

In the photo above my research partner Jada decided that our test needed to be interrupted with kisses, which made things harder for the system to detect my face. 

In theory the accuracy of facial detection could be increased by the following: 

		// Convert the image to grayscale
		Mat gray;
		cvtColor(img, gray, COLOR_BGR2GRAY);

		// Equalize the histogram
		equalizeHist(gray, gray);

---------------------------------------------
## References
  - MIT OpenCourseWare - Lecture 13: Object Detection, Recognition and Pose Determination, PatQuick - https://www.youtube.com/watch?v=lVfm6C51t_Y&list=PLUl4u3cNGP63pfpS1gV5P9tDxxL_e4W8O&index=13
  - Nicolai Nielsen: Object Detection Made Easy: Haar Cascade Classifier Tutorial with OpenCV C++ - https://www.youtube.com/watch?v=oGkxJQ9SB8M
  - Murtaza's Workshop: LEARN OPENCV C++ in 4 HOURS - https://www.youtube.com/watch?v=2FYm3GOonhk
