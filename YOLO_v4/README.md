# YOLOv4: Optimal Speed and Accuracy of Object Detection :- 

Pytorch implementation of YOLO v4 .

## Abstract :- 

There are a huge number of features which are said to
improve Convolutional Neural Network (CNN) accuracy.
Practical testing of combinations of such features on large
datasets, and theoretical justification of the result, is required. Some features operate on certain models exclusively
and for certain problems exclusively, or only for small-scale
datasets; while some features, such as batch-normalization
and residual-connections, are applicable to the majority of
models, tasks, and datasets. We assume that such universal
features include Weighted-Residual-Connections (WRC),
Cross-Stage-Partial-connections (CSP), Cross mini-Batch
Normalization (CmBN), Self-adversarial-training (SAT)
and Mish-activation. We use new features: WRC, CSP,
CmBN, SAT, Mish activation, Mosaic data augmentation,
CmBN, DropBlock regularization, and CIoU loss, and combine some of them to achieve state-of-the-art results: 43.5%
AP (65.7% AP50) for the MS COCO dataset at a realtime speed of ∼65 FPS on Tesla V100. 

## General Object Detection Architecture :- 

![2021-09-20](https://user-images.githubusercontent.com/76057253/133957305-b6883365-5303-4f2c-9ffe-81d435a0215d.png)

Yolo v4 is an single stage detector .
Yolo v4 consists of :- 

BackBone :- CSPDarkNet
CSP net :- 

![image](https://user-images.githubusercontent.com/76057253/133957688-836093e3-a1f4-4d4d-9fc8-80f523d1dc6b.png)

Darknet :- 

![image](https://user-images.githubusercontent.com/76057253/133957736-ba03900c-913f-419c-80ae-5c8bca5d5a11.png)


Neck :- PAN Net 

![image](https://user-images.githubusercontent.com/76057253/133957754-9e75eea7-29fe-4871-9ea1-83933b6ef288.png)

Head :- YOLO v3 

![image](https://user-images.githubusercontent.com/76057253/133957764-37dcfc7c-23d3-4281-8db9-5373dbd478c2.png)

Yolo v3's only head part is used in YOLO v4

Because Yolo v4 is an single stage detector it produces only Dense Predictions . But due to single stage in nature it is faster than RCNN Family .

## YOLO v4 modifications :- 


### Modification to Spatial Attention Module :- 

![2021-09-20 (3)](https://user-images.githubusercontent.com/76057253/133957498-278d23dd-b832-48e0-8952-7de4f6d2f5ab.png)

### Modification to PAN Net :- 

![2021-09-20 (4)](https://user-images.githubusercontent.com/76057253/133957516-2a8106ac-61ef-439b-8c26-2cdee0e02cd1.png)


## YOLO v4 Results :- 

![image](https://user-images.githubusercontent.com/76057253/133957567-d154cb0d-a627-4c8d-b331-76639cdc5243.png)

![image](https://user-images.githubusercontent.com/76057253/133957582-a135b829-9360-4231-a2f2-ea7f032944ea.png)


```
@misc{bochkovskiy2020yolov4,
      title={YOLOv4: Optimal Speed and Accuracy of Object Detection}, 
      author={Alexey Bochkovskiy and Chien-Yao Wang and Hong-Yuan Mark Liao},
      year={2020},
      eprint={2004.10934},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
