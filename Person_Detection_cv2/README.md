# Introduction:
This script for real-time object detection using a pre-trained TensorFlow Hub model.

# About Project:
> Tittle: Object Detection 
* what is Object Detection ?
* What is Object Tracking ?
* Tensorflow Model Hub.
* Model : Efficientdet_lite2_detection
* cv2
* Working
* Requirements
* Conclusion
# what is Object Detection ?
Object detection is a computer vision technique for locating instances of objects in images or videos. Object detection algorithms typically leverage machine learning or deep learning to produce meaningful results. 
* When humans look at images or video, we can recognize and locate objects of interest within a matter of moments. The goal of object detection is to replicate this intelligence using a computer.
* Object detection is a key technology behind advanced driver assistance systems (ADAS) that enable cars to detect driving lanes or perform pedestrian detection to improve road safety. Object detection is also useful in applications such as video surveillance or image retrieval systems.
![](https://in.mathworks.com/discovery/object-detection/_jcr_content/mainParsys3/discoverysubsection/mainParsys3/image.adapt.full.medium.jpg/1655457521805.jpg)

# What is Object Tracking ?
Object tracking means estimating the state of the target object present in the scene from previous information.

![](https://miro.medium.com/v2/resize:fit:600/1*Ty5Wa9vkoZmzN8XT41gVew.gif)

On a high level of abstraction, there are mainly two levels of object tracking.

* Single Object Tracking(SOT)
* Multiple Object Tracking(MOT).
* For more info : [Object Tracking - info](https://medium.com/visionwizard/object-tracking-675d7a33e687)
# Tensorflow Model Hub.
TensorFlow Hub is an open repository and library for reusable machine learning. The tfhub. dev repository provides many pre-trained models: text embeddings, image classification models, TF. js/TFLite models and much more.
# Model : Efficientdet_lite2_detection
EfficientDet-Lite2 Object detection model (EfficientNet-Lite2 backbone with BiFPN feature extractor, shared box predictor and focal loss), trained on COCO 2017 dataset, optimized for TFLite, designed for performance on mobile CPU, GPU, and EdgeTPU.
[Model link](https://tfhub.dev/tensorflow/lite-model/efficientdet/lite2/detection/metadata/1)
# cv2
OpenCV (Open Source Computer Vision Library) is a library of programming functions mainly for real-time computer vision.[1] Originally developed by Intel, it was later supported by Willow Garage, then Itseez (which was later acquired by Intel[2]). The library is cross-platform and licensed as free and open-source software under Apache License 2. Starting in 2011, OpenCV features GPU acceleration for real-time operations.
[For more info](https://en.wikipedia.org/wiki/OpenCV)
# Working:
1. The script loads a pre-trained object detection model from TensorFlow Hub, which is the EfficientDet-Lite2 model.
2. It loads a set of object labels from a CSV file and prepares them for use in the script.
3. It initializes a video capture object to read frames from the default camera.
4. It enters a loop to continuously read frames from the camera and perform object detection on each frame.
5. For each frame, it resizes the image to a fixed size of 512x512 and converts it to RGB format.
6. It converts the image to a tensor and adds an extra dimension to it, since the object detection model expects a batch of images as input.
7. It passes the tensor through the object detection model to obtain the predicted bounding boxes, scores, and labels for the objects in the image.
8. It extracts the relevant information from the model output, including the predicted labels, boxes, and scores.
9. It loops through the predicted labels, boxes, and scores and draws a bounding box and label text on the image for each detected object with a score above a certain threshold.
10. It displays the resulting image with bounding boxes and labels overlaid on the original frame.
11. The loop continues until the user presses the "q" key to quit the script, at which point the video capture object is released and the script ends.
12. Overall, this code performs real-time object detection using a pre-trained model and provides a simple example of how to use TensorFlow Hub for this task.
 
# Conclusion
Essential needs and understanding of Cv2 and Tensorflow lite to build models and application for mobile devices and throw these implementation got exposure to tflite and cv2.