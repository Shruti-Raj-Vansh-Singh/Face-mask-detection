# Face-mask-detection
In this project we will try to detect whether a person is wearing a face mask or not. We will draw a bounding box around the faces of people that are seen in the
image and mark it as masked or unmasked.

For this we will be using YOLOv5, ie, You Only Look Once algo. It is an object detection algorithm that provides us a bounding box and a label on the object in the image. 


What we need to do is to train our model on our own dataset. The dataset that I have used here is [Face Mask Detection](https://www.kaggle.com/andrewmvd/face-mask-detection) One of the biggest task here is to prepare our data for YOLOv5, ie, in the darknet format. For that each image should have a corrersponding .txt file that has the following information

(object class) (x) (y) (width) (height)
where x and y are the coordinates of the center of the bounding box.

For this i used [Roboflow](https://roboflow.com/) where we easily change annotations.

NOTE: You need to generate a data.yaml file.
