# Facial Landmark Detection 

# Overview
In this we will find the facial landmarks, such as eyes, nose, mouth, ears, jaw-line using the popular [dlib](http://dlib.net/) library

![Alt](https://github.com/vaibhavhariaramani/Facial-Landmarks-Detection-with-DLIB/blob/master/1_mArsPXT2PB19dF4sPR-VSA.jpeg)
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
# Usage
 ```
 python facelandmarkdetect.py --shape-predictor shape_predictor_68_face_landmarks.dat --image images/face1.jpg
```
```
$ python facial_landmarks.py --shape-predictor shape_predictor_68_face_landmarks.dat --image <imagefilename>
```

If you wish to output individual detections for facial landmarks (mouth, eyes, nose, jaw, left and right eyebrows):
```
$ python facial_landmarks.py --shape-predictor shape_predictor_68_face_landmarks.dat --image <imagefilename> --draw
```
