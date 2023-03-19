# AnalogClockReader
Reading time based on a photo of an analog clock.
Using computer vision methods and openCV library, I have managed to read the time of an analog clock from a picture.
There were 6 steps:
1. Image processing - Reading the image and converting it to a grayscale representation.
2. Detect clock's frame - Using HoughCircles, and Canny's edge detection algorithm, I detected the clock's frame.
3. Cropping & Resizing - Cropping the image based on its radius and center point, and resizing it to a uniform size.
4. Contours detection - Detecting the hands contours. Doing so with findContours method.
5. Extracting and screening the lines - Create lines to represents the hands, screen duplicated lines and centralizing them. 
                                        Sorting lines by length and assigning roles based on the length.
6. Time calculation - Based on the angles of the lines.
