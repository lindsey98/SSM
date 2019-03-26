# SSM

**<a href="https://arxiv.org/pdf/1803.09867.pdf">Towards Human-Machine Cooperation: Self-supervised Sample Mining for Object Detection</a>**

<a href="http://kezewang.com">Keze Wang</a>,
<a href="https://yanxp.github.io">Xiaopeng Yan</a>,
Dongyu Zhang,
<a href="http://www4.comp.polyu.edu.hk/~cslzhang/">Lei Zhang</a>,
<a href="http://www.linliang.net/">Liang Lin</a>

Sun Yat-Sen University, Presented at [CVPR2018](https://arxiv.org/pdf/1803.09867.pdf)	

<p align=center><img width="80%" src="tools/ssm.png"/></p>

### License

For Academic Research Use Only!

### Citing SSM

If you find SSM useful in your research, please consider citing:

    @InProceedings{Wang_2018_CVPR,
              author = {Wang, Keze and Yan, Xiaopeng and Zhang, Dongyu and Zhang, Lei and Lin, Liang},
              title = {Towards Human-Machine Cooperation: Self-Supervised Sample Mining for Object Detection},
              booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
              month = {June},
              year = {2018}
            }

### Dependencies 

The code is built on top of R-FCN. Please carefully read through [py-R-FCN](https://github.com/YuwenXiong/py-R-FCN) and make sure py-R-FCN can run within your enviornment.

### Datasets/Pre-trained model

1. In our paper, we used Pascal VOC2007/VOC2012 and COCO as our datasets, and ResNet-101 model as our pre-trained model.

2. Please download ImageNet-pre-trained ResNet-101 model manually, and put them into $SSM_ROOT/data/imagenet_models

### Usage

1. training

    Before training, please prepare your dataset and pre-trained model and store them in the right path as R-FCN.
You can go to ./tools/ and modify train_net.py to reset some parameters.Then, simply run sh ./train.sh.

2. testing

    Before testing, you can modify test.sh to choose the trained model path, then simply run sh ./test.sh to get the evaluation result.

### Misc

Tested on Ubuntu 14.04 with a Titan X GPU (12G) and Intel(R) Xeon(R) CPU E5-2623 v3 @ 3.00GHz.

### Acknowledgement 

Thank for the contribution of [Xiaoxi Wang](http://www.sysu-hcp.net/home/).
