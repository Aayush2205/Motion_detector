# Motion_detector
it  detects any motion that happens in the frame and mark it with a green square box . It also take note of the time of start and end of the motion.

## Libraries Used-
**cv2**
**pandas**
**time**
**datetime**

basically this program takes a basic background and then it detects any change in the background that happens in the frame and mark it with green borders. It compares the background with the new motion and the difference we get is the grayscale where the light areas implies that there is motion and the black arear implies there is no motion.

then we use the threshold frame in which if the intensity of the change is near 100 we convert those pixels to a white pixel after getting the threshold we gets the contours around the image then we'll say that if the area of the contour is more than 500 then the object is consider to be moving according to which we'll draw a rectangle around the objects.

we use the functions that are present in cv2 to form the gray frame, delta frame, color frame and the threshold frame.

To exit the kernel and stop the running of the program we've assigned keyword 'q' to pull us out of the result.

we use the datetime.now function to store the start and end time of the object that enters the frame and exits the frame and store it into a .csv file.
