# YOLO9000: Better, Faster, Stronger :- 

Pytorch implementation of YOLO v2 .

YOLOv2 has numerous improvements over YOLOv1. At 67 FPS, YOLOv2 gets 76.8% mAP on PASCAL VOC 2007. At 40 FPS, YOLOv2 gets 78.6% mAP which is better than Faster R-CNN using ResNet and SSD. With such good results, YOLOv2 is published in 2017 CVPR and got over 1000 citations . 
In this paper authors (Joseph Redmon , Ali Farhadi) used anchors boxes .

## Abstract :- 
We introduce YOLO9000, a state-of-the-art, real-time
object detection system that can detect over 9000 object
categories. First we propose various improvements to the
YOLO detection method, both novel and drawn from prior
work. The improved model, YOLOv2, is state-of-the-art on
standard detection tasks like PASCAL VOC and COCO. Using a novel, multi-scale training method the same YOLOv2
model can run at varying sizes, offering an easy tradeoff
between speed and accuracy. At 67 FPS, YOLOv2 gets
76.8 mAP on VOC 2007. At 40 FPS, YOLOv2 gets 78.6
mAP, outperforming state-of-the-art methods like Faster RCNN with ResNet and SSD while still running significantly
faster. Finally we propose a method to jointly train on object detection and classification. Using this method we train
YOLO9000 simultaneously on the COCO detection dataset
and the ImageNet classification dataset. Our joint training
allows YOLO9000 to predict detections for object classes
that don’t have labelled detection data. We validate our
approach on the ImageNet detection task. YOLO9000 gets
19.7 mAP on the ImageNet detection validation set despite
only having detection data for 44 of the 200 classes. On the
156 classes not in COCO, YOLO9000 gets 16.0 mAP. But
YOLO can detect more than just 200 classes; it predicts detections for more than 9000 different object categories. And
it still runs in real-time.


## Architecture :- 
![image](https://user-images.githubusercontent.com/76057253/133395183-b9fc82fc-c6c4-4861-944e-088785ef6777.png)
Authors of YOLO v2 used Darknet as a backbone in YOLO v2 . This model is anchor based model so the output is related to the anchor [batch size , num of anchors , S , S , num classes + 5] .

## Results :- 

YOLO v2 famous video by authors :- 


[![YOLO v2](http://img.youtube.com/vi/VOC3huqHrss/0.jpg)](http://www.youtube.com/watch?v=VOC3huqHrss "YOLO v2 ")

![image](https://user-images.githubusercontent.com/76057253/133397447-ce845955-bea2-4936-8c93-30e1366e2914.png)


```
@misc{redmon2016yolo9000,
      title={YOLO9000: Better, Faster, Stronger}, 
      author={Joseph Redmon and Ali Farhadi},
      year={2016},
      eprint={1612.08242},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```




