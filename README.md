# MTCNN face detection and alignment

## Introduction

  This is a python/mxnet implementation of [Zhang](https://kpzhang93.github.io/)'s work **<Joint Face Detection and Alignment using Multi-task Cascaded Convolutional Neural Networks>**. it's fast and accurate,  see [link](https://github.com/kpzhang93/MTCNN_face_detection_alignment). 

  It should have **almost** the same output with the original work,  for mxnet fans and those can't afford matlab :)


## Environment

-   Python 2.7 
-   Ubuntu 18.04
-   Mxnet-cu90 (=1.3.0)

## Testing

-   Use `python main.py` to test this detection and alignment method.

-   You can change `ctx` to `mx.gpu(0)` to use GPU for faster detection.


see `mtcnn_detector.py` for the details about the parameters. this function use [dlib](http://dlib.net/)'s align strategy, which works well on profile images :) 

## Results

![Detetion Results](https://raw.githubusercontent.com/deepinx/MTCNN_face_detection/master/detection_result.png)



## License

MIT LICENSE



## Reference
```
@article{Zhang2016Joint,
  title={Joint Face Detection and Alignment Using Multitask Cascaded Convolutional Networks},
  author={Zhang, Kaipeng and Zhang, Zhanpeng and Li, Zhifeng and Yu, Qiao},
  journal={IEEE Signal Processing Letters},
  volume={23},
  number={10},
  pages={1499-1503},
  year={2016},
}
```
