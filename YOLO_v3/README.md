# YOLOv3: An Incremental Improvement :- 

Pytorch implementation of YOLO v3 .
YOLO v3 uses multi scaled output to detect small as well as large objects . 

## Abstract :- 
We present some updates to YOLO! We made a bunch
of little design changes to make it better. We also trained
this new network that’s pretty swell. It’s a little bigger than
last time but more accurate. It’s still fast though, don’t
worry. At 320 × 320 YOLOv3 runs in 22 ms at 28.2 mAP,
as accurate as SSD but three times faster. When we look
at the old .5 IOU mAP detection metric YOLOv3 is quite
good. It achieves 57.9 AP50 in 51 ms on a Titan X, compared to 57.5 AP50 in 198 ms by RetinaNet, similar performance but 3.8× faster.


## Architecture :- 
![image](https://user-images.githubusercontent.com/76057253/133398389-378042df-e57b-459c-8abd-2f4f7aaa3a96.png)

YOLO v3 uses Darknet as a backbone architecture and then on top of darknet they are using multi scaled output .

## Results :- 

![image](https://user-images.githubusercontent.com/76057253/133398712-bd957480-4ba8-45a6-9632-eb232f02297c.png)


```
@misc{redmon2018yolov3,
      title={YOLOv3: An Incremental Improvement}, 
      author={Joseph Redmon and Ali Farhadi},
      year={2018},
      eprint={1804.02767},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
