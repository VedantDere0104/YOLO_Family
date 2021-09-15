# You Only Look Once: Unified, Real-Time Object Detection :- 

Pytorch implementation of YOLO v1 .

Before the invention of YOLO, object detector CNNs such R-CNN used Region Proposal Networks (RPNs) first to generate bounding box proposals on the input image, then run a classifier on the bounding boxes and finally apply post-processing to eliminate duplicate detections as well as refine the bounding boxes. Individual stages of the R-CNN network had to be trained separately. R-CNN network was hard to optimize as well as slow.
Creators of YOLO were motivated to design a single stage CNN that could be trained end to end, was easy to optimize and was real-time.

## Abstract :- 

We present YOLO, a new approach to object detection.
Prior work on object detection repurposes classifiers to perform detection. Instead, we frame object detection as a regression problem to spatially separated bounding boxes and
associated class probabilities. A single neural network predicts bounding boxes and class probabilities directly from
full images in one evaluation. Since the whole detection
pipeline is a single network, it can be optimized end-to-end
directly on detection performance.
Our unified architecture is extremely fast. Our base
YOLO model processes images in real-time at 45 frames
per second. A smaller version of the network, Fast YOLO,
processes an astounding 155 frames per second while
still achieving double the mAP of other real-time detectors. Compared to state-of-the-art detection systems, YOLO
makes more localization errors but is less likely to predict
false positives on background. Finally, YOLO learns very
general representations of objects. It outperforms other detection methods, including DPM and R-CNN, when generalizing from natural images to other domains like artwork.

## Conceptual Design :- 
![1_YuYhnVyxRiid6EJwTbsUDg](https://user-images.githubusercontent.com/76057253/133391868-f338b2b5-7cfa-4039-904f-ecc28522cdb8.png)

YOLO divides the input image into S x S grid cells. Each grid cell predicts B bounding boxes and an “objectness” score P(Object) indicating whether the grid cell contains an object or not. Each grid cell also predicts the conditional probability P(Class | Object) of the class the object contained by the grid cell belongs to.



## YOLO v1 Architecture :- 
![1_MwheKv2NXqvbOrWOiAlPrA](https://user-images.githubusercontent.com/76057253/133391660-d681c107-340c-43ce-99d4-278e084a8730.png)


Dataset :- 
https://www.kaggle.com/dataset/734b7bcb7ef13a045cbdd007a3c19874c2586ed0b02b4afc86126e89d00af8d2

## Results :- 
![2021-09-15 (1)](https://user-images.githubusercontent.com/76057253/133392533-4a136ed1-4e5a-4db3-ac7c-cce9fc7066d9.png)

![2021-09-15 (2)](https://user-images.githubusercontent.com/76057253/133393023-5b272eca-8c73-490f-8683-711fbe5bfad7.png)


```
@misc{redmon2016look,
      title={You Only Look Once: Unified, Real-Time Object Detection}, 
      author={Joseph Redmon and Santosh Divvala and Ross Girshick and Ali Farhadi},
      year={2016},
      eprint={1506.02640},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
