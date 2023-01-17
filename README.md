# Object-Detection-Using-Faster-R-CNN

A Basic Implementation of paper https://arxiv.org/pdf/1506.01497.pdf on Faster R-CNN to develop a more accurate and faster Neural Network for Object Detection.


# Dataset Used

Open Images Dataset V6

https://storage.googleapis.com/openimages/web/index.html

# Model Structure
![Alt text](https://miro.medium.com/max/1095/1*jYDMaYeH-TrcoofDqCdxug.jpeg)


The Above Shown Model uses a VGG network to get the feature maps of the Input image, these feature maps are then provided to the RPN (Region Proposal Network). The RPN has two different layers one provides the bounding boxes and one provides the region proposals. These proposals are then sent into a ROI Pooling Layer which converts all the Region Proposals into a 7X7 shaped proposals. These fixed shape proposals are then feeded into a final set of layers which provides the class of the object and adjusts the bounding boxes around the object.


# Advantages of Faster RCNN over Other Neural Networks
In terms of Detection time, Faster R-CNN is faster than both R-CNN and Fast R-CNN. The Faster R-CNN also has better mAP than both the previous ones.
It Can Be Trained End To End Unlike R-CNN which has Indivisual Components and Proposals are needed to be Feed Each time.
