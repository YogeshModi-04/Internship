# Introduction:
Hi there, I am Yogesh Modi and I have being working on DeepFake Image detection project indivually as Jr.Data Science intern at Zummit infolabs and with the help of my mentor, I was able to complete this project.

# About Project:
> Tittle:  DeepFake Image detection :
* What is Deepfakes ?
* How its detects Deepfakes images ?
* Uses Tensorflow Data-pipeline APIs
* Model used : CNN.
* Image Classification
* Model accurcy 99%
* Conclusion

## What is Deepfakes ?

* Deepfakes are falsely created or computer genrated images or videos using Auto-Encoder or GANs are widely used in Entertainment Industries and there are two types of Deepfakes.

 1. Face Swaps.
  * In this type of Deepfakes images are bound to a feartuers sets of any perticular video of choice and either you are using Auto-Encoder or GANs it maps those featuers of video to that image and make it animate.

 2. Puppetry.
 * In this type of Deepfake we swaps faces form videos and mimic the feature sets of those videos to match there expression.

## CNN:
* A convolutional neural network, or CNN, is a deep learning neural network sketched for processing structured arrays of data such as portrayals.
* CNN are very satisfactory at picking up on design in the input image, such as lines, gradients, circles, or even eyes and faces.
* This characteristic that makes convolutional neural network so robust for computer vision.
* CNN can run directly on a underdone image and do not need any preprocessing.
* A convolutional neural network is a feed forward neural network, seldom with up to 20.
* The strength of a convolutional neural network comes from a particular kind of layer called the convolutional layer.
* CNN contains many convolutional layers assembled on top of each other, each one competent of recognizing more sophisticated shapes.
* With three or four convolutional layers it is viable to recognize handwritten digits and with 25 layers it is possible to differentiate human faces.
* The agenda for this sphere is to activate machines to view the world as humans do, perceive it in a alike fashion and even use the knowledge for a multitude of duty such as image and video recognition, image inspection and classification, media recreation, recommendation systems, natural language processing, etc.
![CNN](https://miro.medium.com/max/1400/1*uAeANQIOQPqWZnnuH-VEyw.jpeg)

## TensorFlow Datapipe-Line API:
* The tf.data API introduces a tf.data.Dataset abstraction that represents a sequence of elements, in which each element consists of one or more components. For example, in an image pipeline, an element might be a single training example, with a pair of tensor components representing the image and its label.

* There are two distinct ways to create a dataset:

* A data source constructs a Dataset from data stored in memory or in one or more files.

* A data transformation constructs a dataset from one or more tf.data.Dataset objects.
* For More Info : [https://www.tensorflow.org/guide/data]

 ## How its detects Deepfake images ?
 * first if fetches the image from tensorflow dataset.
 * Its uses CNN(Convolution Neural Networks) to train the model.
 * its classify images on set of values that are mismatch from orignal images.
 * values:
 1. Textures.
 2. Background.
 3. Shapes.
 4. Edges.
 5. Pixels




# Requirements:
* Ram : 12 GB+
* Storage: 4+ GB
* Cpu: >= i5 10th GEN
* [Dataset](https://www.kaggle.com/datasets/xhlulu/140k-real-and-fake-faces?resource=download&select=real_vs_fake)

# Conclusion: 
* Get a brief info on Deepfakes, how it is created and how we can detects it and a short intro on GANs, TensroFlow Datapipeline API and Use of it and lastly get more to know about image classification.