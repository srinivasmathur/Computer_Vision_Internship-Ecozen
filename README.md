# Computer_Vision_Internship-Ecozen

## Application of Computer Vision for fruit detection and quality prediction-
  To detect fruits(in this case litchi) in the image, count the number and classify each piece  as fresh or non-fresh.

## Training and running the model:

### Labelling using labellmg:
-------------------------
1)Select the directory where images are present.
2)Make bounding boxes for each object you want to detect(choose only one class,because the model works for only one class).
3)Save the file.
4)Repeat this for all the images present in the directory.
5)Make zip file containing all the images and the txt file.Name the zip file as 'images'
===============================================================================================

### Object detection model using Yolov3:
------------------------------------
1)open the "Train_YoloV3.ipynb" notebook in google colab.
2)click on Edit in the toolbar and click on Notebook setting.Change the Hardware accelerator to GPU.
3)Run the script,it will first mount a google drive. 
4)Upload the images.zip file in the yolov3 folder.
5)It will take 3-4 hrs to train the model.
6)The model will be saved in the yolov3 folder.
================================================================================================

### Quality prediction model:
---------------------------
1)open "Train quality prediction classifier" notebook.
2)Specify the path where test and train images are located.
3)Run the complete code.
4)It will save the model in google drive.
=================================================================================================

### Running object detection and quality prediction model:
--------------------------------------------------------
1)Once the object detection and quality prediction classifier models are trained,download it in a local computer.
2)Open the "Litchi detection and quality prediction.ipynb" notebook.
3)Specify the path for quality prediction classifier model in the variable "model", object detection model in the variable "weightspath" and "yolov3_testing.cfg".
4)Specify the path for images.
5)Run the complete code.It will show the results after every image.
6)Down below,there is a code for cropping the image of each object detected and saving it in a folder.This can be used to generate more dataset for quality prediction.
