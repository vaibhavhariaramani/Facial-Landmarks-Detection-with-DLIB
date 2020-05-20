# Facial Landmark Detection 


# Facial Landmarks Detection with DLIB
### Detects the face landmarks such as nose, eyes, etc. using just Python, OpenCV and dlib

Amazing and easy face landmarks detector with dlib library.
# Overview
In this we will find the facial landmarks, such as eyes, nose, mouth, ears, jaw-line using the popular [dlib](http://dlib.net/) library

for further information checkout my blog: [Facial landmarks with dlib, OpenCV, and Python](https://sites.google.com/view/geeky-traveller/computer-vision/facial-landmarks-detection). 
## **Key Points**
1. Steps involved:
    1. Localize the face in the image
    2. Detect the key facial structures on the face ROI
2. Assumptions:
    1. We already have the trained face detector and face landmark detector.
3. Variety of things the face detector detects:
    1. Nose
    2. Mouth
    3. Left eye
    4. Right eye
    5. Left eyebrow
    6. Right eyebrow
    7. Jaw
4. Data required for training of dlib's facial landmark detector:
    1. Training set of labeled facial landmarks on the image.
    2. Priors: Probability on distance between pairs of input pixels
5. The dlib's face detector is an implementation of **One Millisecond Face Alignment with an Ensemble of Regression Trees** paper by Kazemi and Sullivan (2014).
6. 68 coordinates are detected for the given face by the face detector. The image is shown below.
![Face landmarks coordinates image]
![Alt](https://github.com/vaibhavhariaramani/Facial-Landmarks-Detection-with-DLIB/blob/master/1_mArsPXT2PB19dF4sPR-VSA.jpeg)
7. dlib's framework can be trained to predict any shape. Hence it can be used for custom shape detections as well.
8. Used dlib's pre-trained face detector based on the modification of the standard **Histogram of Oriented Gradients + Linear SVM method** for object detection.
9. The face detector used up-scaling before face detection for better results.
10. This method works even for multiple faces in the image.
# Requirements:

dlib, cv, imutils


# Link:
https://sites.google.com/view/geeky-traveller/computer-vision/facial-landmarks-detection

# Run:
Download the detector model [here](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2)
# Dependencies
You also need shape detector, you can download it by 
```
wget http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2
```
 ## **Commands to run the detection:**
 ```
python facial_landmarks_mine.py --shape-predictor shape_predictor_68_face_landmarks.dat --image images/example_01.jpg
```
```
$ python facial_landmarks.py --shape-predictor shape_predictor_68_face_landmarks.dat --image <imagefilename>
```

If you wish to output individual detections for facial landmarks (mouth, eyes, nose, jaw, left and right eyebrows):
```
$ python facial_landmarks.py --shape-predictor shape_predictor_68_face_landmarks.dat --image <imagefilename> --draw
```
## **Results:**
The results are awesome. We can see pretty accurate face landmark detections.

**Input**
<img src="https://github.com/vaibhavhariaramani/Facial-Landmarks-Detection-with-DLIB/blob/master/input%20images/test4.jpg" width="250"/>**Output**<img src="https://github.com/vaibhavhariaramani/Facial-Landmarks-Detection-with-DLIB/blob/master/output%20images/Output_screenshot_text4.png" width="250"/>


Example input 1      Example output 1

**Input**

![Example input 2](https://github.com/vaibhavhariaramani/Facial-Landmarks-Detection-with-DLIB/blob/master/input%20images/test5.jpg)

**Output**

![Example output 2](https://github.com/vaibhavhariaramani/Facial-Landmarks-Detection-with-DLIB/blob/master/output%20images/Output_screenshot_test5.png)

**Input**

![Example input 3](https://github.com/vaibhavhariaramani/Facial-Landmarks-Detection-with-DLIB/blob/master/input%20images/test6.jpg)

**Output**

![Example output 3](https://github.com/vaibhavhariaramani/Facial-Landmarks-Detection-with-DLIB/blob/master/output%20images/Output_screenshot_test6.png)


# Resources 

To learn more about these Resources you can Refer to some of these articles written by Me:-

https://sites.google.com/view/geeky-traveller/computer-vision/facial-landmarks-detection

### Made with ❤️ by Vaibhav Hariramani
#### About me

I am an Actions on Google, Internet of things, Alexa Skills, and Image processing developer.
I have a keen interest in Image processing and Andriod development.
I am Currently studying at  Chandigarh University, Punjab.

You can find me at:-
[Linkedin](https://www.linkedin.com/in/vaibhav-hariramani-087488186/) or [Github](https://github.com/vaibhavhariaramani) .

Happy coding ❤️ .
