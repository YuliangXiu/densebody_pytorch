# densebody_pytorch
PyTorch implementation of CloudWalk's CVPR 2019 paper [DenseBody](https://arxiv.org/abs/1903.10153v3)


![paper teaser](teaser/teaser.jpg)

### Prerequisites
```
Ubuntu 18.04
CUDA 9.0
Python 3.6
PyTorch 1.0.0
chumpy (For converting SMPL model to basic numpy arrays)
spacepy, h5py (For processing Human36m cdf annotations)
```

(Optional) Install [torch-batched-svd](https://github.com/KinglittleQ/torch-batch-svd) for speedup (Only tested under Ubuntu system).


### TODO List
- [x] Creating ground truth UV position maps for Human36m dataset.
    - [x] [20190329]() Finish UV data processing.
    - [ ] [Proceeding] Align SMPL mesh with input image.
    - [ ] Generate and save UV position map.
- [ ] Finish baseline model training
    - [ ] Testing with several new loss functions.
    - [ ] Testing with different networks.
- [ ] Report 3D reconstruction results.
    - [ ] Setup evaluation protocal and MPJPE-PA metrics.


### Current Progress
Finish UV texture map processing. Here's the result:

![UV_map](SMPL_UV_map.png)

### Citation
Please consider citing the following paper if you find this project useful.
[DenseBody: Directly Regressing Dense 3D Human Pose and Shape From a Single Color Image](https://arxiv.org/abs/1903.10153v3)

### Disclaimer
Please note that this is an unofficial implementation free for non-commercial usage only. For commercial cooperation please contact the original authors.