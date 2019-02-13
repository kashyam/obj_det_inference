# Object Detection Inference App  
  
  
###### [Detect Object with oDetection App](https://odetection.herokuapp.com/)  
  
  
## Oject Detection using OpenCV DNN

Model - [SSD Mobilenet Trained on COCO dataset](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/detection_model_zoo.md)
Applications - OpenCV / Flask
Platform - Heroku  
  
  
  
  
## App.py  
  
  
  
App.py handles the [index.html](https://github.com/kashyam/obj_det_inference/tree/master/templates/index.html) and takes input as images via POST method.  
App.py handles the uploaded image and passes it to the detectObject method of the Detector class. The images with bounding boxes encoded as jpg is converted to bytes and sent to fulfil the http request.  
  
  
  
  
  
## Object Detector.py  
  
  
  
This module uses OpenCV's **cv.dnn.readNetFromTensorflow** to read the frozen inference graph trained with tensorflow in Microsoft COCO Dataset. The image passed through the model and label id, bouding box coordinates and confidence are extracted whicha re used to draw bounding boxes over the detected objects.  
  
  
  
  
## Objects detected using the [odetector App](https://odetection.herokuapp.com/)  
  
  
  ![jpg](/detections/elephant1.jpg)
  
  
  
  
  ![jpg](/detections/elephant2.jpg)
  
  
  
  
  ![jpg](/detections/bench.jpg)
  
  
  
  
  ![jpg](/detections/bird11.jpg)
  
  
  
  
  ![jpg](/detections/bus1.jpg)
  
  
  
  
  ![jpg](/detections/bird2.jpg)
  
  
  
  
  ![jpg](/detections/zebra.jpg)
  
  
  
  
  ![jpg](/detections/car1.jpg)
  
  
  
  
  ![jpg](/detections/car2.jpg)
  
  
  
  
  ![jpg](/detections/carrot.jpg)
  
  
  
  
  ![jpg](/detections/car3.jpg)
  
  
  
  
  ![jpg](/detections/cow1.jpg)
  
  
  
  
  ![jpg](/detections/chair1.jpg)
  
  
  
  
  ![jpg](/detections/cow2.jpg)
  
  
  
  
  ![jpg](/detections/cows3.jpg)

