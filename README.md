# swiftframes
Motion-compensated Frame Interpolation Algorithm using Features Matching

# Warning :
swiftframes is still in an early stage.

# Dependencies :
- Python 3
- Numpy
- OpenCV, preferably with contrib (pip install opencv-contrib-python), but contrib is not mandatory (only needed if you want to try with feature detector and/or descriptors that are only in contrib like sift and surf)
- ffmpeg (or gstreamer) for the video part

# How to use :
You can use :

test.py provides some example code on how to interpolate from some png files.

testVideo.py can be used to generate a interpolated video with double the original framerate.

you can use testVideo.py like that :

python testVideo.py VideoFileName

# Code structure :
the "main" driver functions are in test.py and testVideo.py, since I don't have a real main function yet.
motion.py contains the motion detection algorithm, it uses object from motion_match.py.
interpolation.py contains the current interpolation algorithm.
motion_match and motion_features contain objects used in the process
the util folder contains some utility functions I used.

detector-tests and matching-tests were only used to compare the quality of different features regarding 