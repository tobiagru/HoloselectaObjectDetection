# ObjectDetection
ObjectDetection for Grocery Products

## Explanation
This is part of the Masterthesis:
Title: Real Time Enhancement of Nutrition Data for Groceries with Object Detection and Augmented Reality: Feasibility & Usability Study
Author: Tobias Grundmann
Supervisor: Klaus Fuchs
Tutor: Prof. Elgar Fleisch
Chair: Information Management
Department: Managment, Technology & Economics
University: ETH Zurich
Explanation: This is part of an effort to provide Object detection for any range of groceries to any granularity level. References are the products of the EatFit database (https://eatfit-service.foodcoa.ch/products/).


## Files
* DataHandling.ipynb - Data Pipeline
* Config.json - all configs


##  Ideas
* Add an OCR net (e.g Attention OCR https://github.com/tensorflow/models/tree/master/research/attention_ocr) to the object detection
   * as a seperate part on top of the image patch (rcnn style)
   * as part of the CNN net (faster-rcnn style)
* ...

## Reviews
* Object Detection - https://medium.com/comet-app/review-of-deep-learning-algorithms-for-object-detection-c1f3d437b852
* Object Detection - https://github.com/hoya012/deep_learning_object_detection
* Object Detection - https://arxiv.org/abs/1807.05511v1

## Modelzoos
* Keras Applications – VGG, ResNet, Inception, DenseNet, MobileNet, NASNet - https://keras.io/applications
* Tensorflow Object Detection API - SSD, Faster R-CNN, RetinaNet  – https://github.com/tensorflow/models/tree/master/research/object_detection/models
* Tensorflow Slim - InceptionNet, ResNet, MobileNet, NASNet, PNASNet –  https://github.com/tensorflow/models/tree/master/research/slim
* SSD port to Keras – SSD - https://github.com/pierluigiferrari/ssd_keras
* RetinaNet port to Keras – RetinaNet - https://github.com/fizyr/keras-retinanet
* Yolo v3 Port to Keras – yolo - https://modelzoo.co/model/keras-yolov3
* Collection of Object Detection Nets – all - https://github.com/hoya012/deep_learning_object_detection


