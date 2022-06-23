# Drowsiness-Detection
Drowsiness is defined as a decreased level of awareness portrayed by sleepiness and trouble in staying alarm but the person awakes with simple simple excitement by stimuli.
A computer vision system that can automatically detect person drowsiness in a real-time video stream and then play an alarm If the person appears to be drowsy.
This is done with the help of image processing.
In this I have used face detection and eye detection to check the drowsiness.
I need the SciPy package so we can compute the Euclidean distance between facial landmarks points in the eye aspect ratio calculation.
I also need the imutils package, my series of computer vision and image processing functions to make working with OpenCV easier.
In order to actually play our WAV/MP3 alarm, we need the pygame library, a pure Python, cross-platform implementation for playing simple sounds.
we have to collect 68 total landmarks per frame.
If the eye aspect ratio falls below0.3 threshold, we’ll start counting the number of frames the person has closed their eyes for.
If the number of frames the person has closed their eyes in exceeds
EYE_AR_CONSEC_FRAMES=48
meaning that if a person has closed their eyes for 48 consecutive frames, we’ll play the alarm sound.
ear = (A + B) / (2.0 * C)
Libraries used- from scipy.spatial import distance as dist, from imutils.video import VideoStream ,from imutils import face_utils , from threading import Thread
, import numpy,import playsound,import argparse,imutilstime, dlib ,cv2.
