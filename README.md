# Yolov8-Custom-Object-Detetction
This repos explains the custom object detection training using Yolov8


The goal is to detetc a person is using mask or not and whether using it in wrong way. I am using "Face Mask Dataset" from kaggle which is already available in yolo format. https://www.kaggle.com/datasets/maalialharbi/face-mask-dataset?resource=download

This is a initial version of custom trianing with YOLOv8. Currently YOLOv8 is the newest state-of-the-art YOLO model that can be used for object detection, image classification, and instance segmentation tasks.

I am using Google Colab for trianing. If you are intrested to check custom trianing with YOLOv5, please follow this link 😀 https://github.com/Balakishan77/yolov5_custom_trained_traffic_sign_detector.

### About this Dataset for Detection Tasks:
https://www.kaggle.com/datasets/maalialharbi/face-mask-dataset?resource=download This is ready to use Face Mask Dataset in YOLO format for Detection tasks. It can be used for training as well as for testing. 

##### The images are split as follows:
Test: 136 =10%
Train: 990 = 70%
Valid: 294 = 20%
Total = 1420 images
Image Augmentation was done to increase the dataset size and make it more powerful.
The images are in: JPEG, PNG format

The dataset has 3 classes:
no_mask
mask
improper_mask

### Training Custom Face Mask Detection Model:
I have used Yolov8m for custom training with Face Mask data. I did training in Google colab by reading data from Google drive.
The notebook explains the below steps:

1.Setting Up Google Colab \
2.YOLOV8 Installation \
3.Mounting Google Drive \
4.Create face_mask_detetcion.yaml (dataset config file) (YOLOV8 format) \
5.Training Our Custom Face Mask Detetcion Model \
6.Metrics \
7.Run Inference With Custom YOLOv8 Object Detector Trained Weights


### Inference results on the video using Yolov8 custome trained model:
Attached video as seperate file in repo. Below are the some of the detetcions on image.![vlcsnap-2023-01-13-19h49m04s704](https://user-images.githubusercontent.com/40944675/212341969-e09657c3-5f2c-41f2-8418-210e3cfe474d.png)
![vlcsnap-2023-01-13-19h51m37s155](https://user-images.githubusercontent.com/40944675/212341980-c9e93f14-fc12-47f9-9401-375da11dea7e.png)


![vlcsnap-2023-01-13-19h48m54s744](https://user-images.githubusercontent.com/40944675/212341947-4dbb4ff1-b624-49da-a68b-62b77716eb5f.png)

### **Conclusion:**
Based on the inference results, the trained model is doing a great job. We can still imrpove it by using large yolov8 models, additional data and hyperparameter changes. Model file is also available for any type of testing.
### **References:**

1.https://github.com/ultralytics/ultralytics

2.https://docs.ultralytics.com/tasks/detection/

3.https://www.kaggle.com/datasets/maalialharbi/face-mask-dataset?resource=download
