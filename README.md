# **Custom-Object-Detection-Notebook**
This jupyter notebook trains a TensorFlow 2 custom object detection model. You can choose your own data set to make a model that can recognize those set of images, as long as they are properly labelled.

This jupyter notebook is meant to be run on Google Drive, and using Google Colab as the environment.

---
<br>

## **Before running the notebook, make sure to have the following directories in your  G-Drive.** ##

1.  Create a folder named customTF2 in your google drive.

2. Create another folder named training inside the customTF2 folder (the training folder is where the checkpoints will be saved during training).

3. Create another folder named data inside the customTF2 folder.

4. Create a folder named images for your custom dataset images and create another folder named annotations for its corresponding PASCAL_VOC format labeled XML files.

5. Create their zip files and upload them to the customTF2 folder in your drive.

6. After attaching your drive, your directory should look something like this: 
<img src="assets/directory.png" alt="Colab directory after mounting drive" width="50%">


<br><br>

## **Image annotation to get PASCAL_VOC XML file**
 **Image annotation** is the process of labeling or classifying an image using text, annotation tools, or both, to show the data features you want your model to recognize on its own.
 
 You can check out the [Github repo for LabelImg](https://github.com/heartexlabs/labelImg), or read more about image labeling [here](https://viso.ai/computer-vision/labelimg-for-image-annotation/).


<br><br>

## **ROADMAP TO CREATING AN OBJECT DETECTION TFLITE MODEL**
* Collect the dataset of images and label them to get their xml files.

* Install the TensorFlow Object Detection API.
* Generate the TFRecord files required for training. (need generate_tfrecord.py script and csv files for this)
* Edit the model pipeline config file and download the pre-trained model checkpoint.
* Train and evaluate the model.
* Export and convert the model into TFlite(TensorFlow Lite) format.
* Deploy the TFlite model on Android / iOS / IoT devices.

<br><br>