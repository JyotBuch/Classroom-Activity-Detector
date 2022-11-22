# Classroom-Activity-Detector

![Rubiscape-Logo](https://github.com/JyotBuch/Classroom-Activity-Detector/blob/master/Images/Rubiscape-Logo.png)

- This project is mainly based on detecting the activity in a classroom through the cctv footage.
- There are many situations where the classrooms are left unattended and still need to be monitored to be alerted in case of any misbehaviour 
- So while classrooms are always monitored on CCTV, here we use the benefits of technology to detect certain anomalies in the classroom. This is performed by applying Deep Learning techniques and using it on the CCTV footage


We have used YOLOV5 architecture to train this model for 2 custom classes
 - Standing Up
 - Sitting Down
 
The weights can be downloaded from [here](https://github.com/JyotBuch/Classroom-Activity-Detector/blob/master/weights/best.pt).

In order to work with the weights, we are currently using a simple CLI process where we run a command to process the video footage

Please make sure to clone the YOLOv5 model from [here](https://github.com/ultralytics/yolov5)

Upon downloading the weight files, run the following command in the **YOLOv5** folder

`python detect.py --source <location to video or image> --weights <location to weights file>`

### Evaluation 
Our model is evaluated based on a few charts

#### Confusion Matrix
<img src="https://github.com/JyotBuch/Classroom-Activity-Detector/blob/master/Images/confusion_matrix.png" width="600" height="400" />

#### Precision Metrics
<img src="https://github.com/JyotBuch/Classroom-Activity-Detector/blob/master/Images/accuracy.png" width="800" height="400" />


### Results
![gif](https://github.com/JyotBuch/Classroom-Activity-Detector/blob/master/Images/classroom-gif.gif)
