# YOLO With IOU Losses :- 

Pytorch implementation of YOLO with IOU losses like IOU Loss , GIOU Loss , DIOU Loss , CIOU Loss

Abstract :- 
In present object detection systems, the deep convolutional
neural networks (CNNs) are utilized to predict bounding
boxes of object candidates, and have gained performance advantages over the traditional region proposal methods. However, existing deep CNN methods assume the object bounds
to be four independent variables, which could be regressed
by the 2 loss separately. Such an oversimplified assumption
is contrary to the well-received observation, that those variables are correlated, resulting to less accurate localization.
To address the issue, we firstly introduce a novel Intersection
over Union (IoU) loss function for bounding box prediction,
which regresses the four bounds of a predicted box as a whole
unit. By taking the advantages of IoU loss and deep fully
convolutional networks, the UnitBox is introduced, which
performs accurate and efficient localization, shows robust to
objects of varied shapes and scales, and converges fast. We
apply UnitBox on face detection task and achieve the best
performance among all published methods on the FDDB
benchmark.


```
@article{Yu_2016,
   title={UnitBox},
   ISBN={9781450336031},
   url={http://dx.doi.org/10.1145/2964284.2967274},
   DOI={10.1145/2964284.2967274},
   journal={Proceedings of the 24th ACM international conference on Multimedia},
   publisher={ACM},
   author={Yu, Jiahui and Jiang, Yuning and Wang, Zhangyang and Cao, Zhimin and Huang, Thomas},
   year={2016},
   month={Oct}
}
```

```
@misc{zheng2019distanceiou,
      title={Distance-IoU Loss: Faster and Better Learning for Bounding Box Regression}, 
      author={Zhaohui Zheng and Ping Wang and Wei Liu and Jinze Li and Rongguang Ye and Dongwei Ren},
      year={2019},
      eprint={1911.08287},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
