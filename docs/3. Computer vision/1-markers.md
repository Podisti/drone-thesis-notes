# Markers

## ArUcO Markers
Special markers, which are part of the OpenCV library, and in Gazebo (aruco world).  
They are designed to be easily detectable, and to easily extract orientation from the image.
They hold minimal information, which is not necessarily a problem 
[OpenCV detection tutorial](https://docs.opencv.org/3.4/d5/dae/tutorial_aruco_detection.html)

## April tags
Designed for easy detection even in bad conditions. Easily recognizable even with low resolution, which enables fast processing.  
[Reference](https://docs.wpilib.org/en/stable/docs/software/vision-processing/apriltag/apriltag-intro.html)  

“designed to be automatically detected and localized even when it is at very low resolution, unevenly lit, oddly rotated, or tucked away in the corner of an otherwise cluttered image”
[AprilTag: A robust and flexible visual fiducial system](https://docs.wpilib.org/en/stable/_downloads/50ad8f5c37aa2b4f174a3fde0fd71137/olson2011tags.pdf)  
[AprilTag 2: Efficient and robust fiducial detection](https://docs.wpilib.org/en/stable/_downloads/cba1039fecb1731ad4e233f7638b9fd0/wang2016iros.pdf)

## QR Codes
Usable, but hold unnecessarily amount of data. // TODO  
[OpenCV tutorial](https://learnopencv.com/opencv-qr-code-scanner-c-and-python/)

## Classic H
No implemented functionality to detect it. Therefore if the drone was landing on an H, it would need custom code for detecting it.

## Nested tags
Nesting tags is done by printing a smaller tag inside a big one. This is done to improve detection of the landing pad, and increase accuracy, because once the drone can't see most of the tag, it is no longer making adjustments to land more precisely. The smaller tag gives the drone a precise point which it can see until it lands.