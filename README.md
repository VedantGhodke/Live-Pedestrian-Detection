# Live Pedestrian Detection Using Python and TensorFlow

This project is developed using TensorFlow to detect the number of pedestrians entering a building complex. 

### Python Packages Needed:

* You must have pip and Python pre-installed
* <a href='https://github.com/tensorflow/tensorflow'>TensorFlow</a><br>
* <a href='https://github.com/skvark/opencv-python'>OpenCV</a><br>


## Installation instructions:

``` bash
# For CPU
pip install tensorflow
# For GPU
pip install tensorflow-gpu
```
For Ubuntu
``` bash
sudo apt-get install protobuf-compiler
```
For OSX
```
brew install protobuf
```
Other Libraries
```
pip install opencv-python
```
Tensorflow object detection API
```
protoc utils/*.proto --python_out=.
```

## Running
If you want to test out the implementation then you can use the person_detection_every_sec.py which is working on pre recorded video<br/>
```
python person_detection_every_sec.py
```

### Instruction to plot bounding boxes
As per the original implementation of the tensorflow object detection API, the bounding boxes are normalised. To get the original dimensions you need to do the following.

```
(left, right, top, bottom) = (xmin * im_width, xmax * im_width,
                              ymin * im_height, ymax * im_height)
```
