# FACE_DETECTION

<h2>Introduction:</h2>
<p>Face detection is a computer technology being used in a variety of applications that identifies human faces in digital images. Face detection can be regarded as a specific case of object-class detection. In object-class detection, the task is to find the locations and sizes of all objects in an image that belong to a given class. Examples include upper torsos, pedestrians, and cars.</p>
<p>Face-detection algorithms focus on the detection of frontal human faces. It is analogous to image detection in which the image of a person is matched bit by bit. Image matches with the image stores in the database.</p>

<h4>Before</h4> 
--image smile.jpg



After








How face detection works: 
Face detection applications use algorithms and ML to find human faces within larger images, which often incorporate other non-face objects such as landscapes, buildings and other human body parts like feet or hands. Face detection algorithms typically start by searching for human eyes -- one of the easiest features to detect. The algorithm might then attempt to detect eyebrows, the mouth, nose, nostrils and the iris. Once the algorithm concludes that it has found a facial region, it applies additional tests to confirm that it has, in fact, detected a face.
Design Solution: 

 Problem Statement :
           	Many parts of a certain image may not contain the useful information we need, so the goal of face detection is to display an image that can be identified as human faces and can be analyzed more easily. 










Requirements:
•	OpenCV
Importing the Libraries:
•	CV2
•	HAAR Cascade

 Algorithm:
	Steps in Face detection:
1.Importing the picture
import cv2 as cv
Building the model
#Read the image
 img = cv.imread('smile.jpg')
 
2.Haar cascade model
Face_model = cv.CascadeClassifier(face-detect-model)
 
3.Change color BGR to GRAY
gray_scale = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
 
4.Draw a square
cv.rectangle(img, (200,200), (400,400), (255,255,0), 2) #RGB -> BGR






for (x,y,w,h) in faces:

5.Draw a square like in the beginning.
cv.rectangle(img, (x,w), (y,h),(x+w,y+h), (255,255,0), 2) 	#RGB to BGR






6.Window at will be pop up
cv.imshow('image', img)
 
7.Exit and turn off window
 cv.waitkey(0)
cv.destroyAllWindows()


Conclusion:
Face detection is a type of computer technology used in various applications to accurately identify faces in images and in specific cases of face detection Its task is to find the location and all objects in a given class image and will focus on detecting human faces.

