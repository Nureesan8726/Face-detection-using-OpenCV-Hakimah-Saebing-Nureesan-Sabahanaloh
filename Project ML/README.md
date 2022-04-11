# FACE_DETECTION

<h2>Introduction:</h2>
<p>Face detection is a computer technology being used in a variety of applications that identifies human faces in digital images. Face detection can be regarded as a specific case of object-class detection. In object-class detection, the task is to find the locations and sizes of all objects in an image that belong to a given class. Examples include upper torsos, pedestrians, and cars.</p>
<p>Face-detection algorithms focus on the detection of frontal human faces. It is analogous to image detection in which the image of a person is matched bit by bit. Image matches with the image stores in the database.</p>

<h4>Before</h4> 
<img src="smile.jpg">
<h4>After</h4>
<img src="smile2.jpgg">


<h2>How face detection works:</h2>
<p>Face detection applications use algorithms and ML to find human faces within larger images, which often incorporate other non-face objects such as landscapes, buildings and other human body parts like feet or hands. Face detection algorithms typically start by searching for human eyes -- one of the easiest features to detect. The algorithm might then attempt to detect eyebrows, the mouth, nose, nostrils and the iris. Once the algorithm concludes that it has found a facial region, it applies additional tests to confirm that it has, in fact, detected a face.</p>

<h2>Design Solution:</h2>
<img src="capture11.png">

<h2>Problem Statement :</h2>
<p>Many parts of a certain image may not contain the useful information we need, so the goal of face detection is to display an image that can be identified as human faces and can be analyzed more easily.</p>

<h2>Requirements:</h2>
<p>• OpenCV</p>

<h2>Importing the Libraries:</h2>
<p>• CV2</p>
<p>• HAAR Cascade</p>

 <h2>Algorithm:</h2>
<h4><p>>Importing the picture</p></h4>
<p> Import cv2 as cv</p>
<p> Building the model</p>

<h4><p>>Read the image</p></h4>
 <p>img = cv.imread('smile.jpg')</p>
 
<h4><p>>Haar cascade model</h4></P>
<p>Face_model = cv.CascadeClassifier(face-detect-model)</p>
 
<h4><p>>Change color BGR to GRAY</h4></P>
<p>gray_scale = cv.cvtColor(img, cv.COLOR_BGR2GRAY)</p>
 
<h4><p>>Draw a square</h4></P>
<p>cv.rectangle(img, (200,200), (400,400), (255,255,0), 2) #RGB -> BGR</p>
<p>for (x,y,w,h) in faces:</p>

<h4><p>>Draw a square like in the beginning.</h4></P>
<p>cv.rectangle(img, (x,w), (y,h),(x+w,y+h), (255,255,0), 2) 	#RGB to BGR</p>

<h4><p>>Window at will be pop up</h4></P>
<p>cv.imshow('image', img)</p>
 
<h4><p>>Exit and turn off window</h4></P>
 <p>cv.waitkey(0)</p>
 <p>cv.destroyAllWindows()</p>


<h2>Conclusion:</h2>
<p>Face detection is a type of computer technology used in various applications to accurately identify faces in images and in specific cases of face detection Its task is to find the location and all objects in a given class image and will focus on detecting human faces.</p>

