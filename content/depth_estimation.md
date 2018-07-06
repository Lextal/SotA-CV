# Monocular depth estimation

## Description

Dense regression problem of reconstructing a pixel-wise depth map from a single image.

Main evaluation metric used here is Root Mean Square Error (RMSE).


## Results

### KITTI < 50 m.

Max depth is restricted to 50 meters.

[Dataset description](datasets/kitti_depth_estimation.md)

| Model | Score | Weights | Paper | Code |
|:------|:-----:|:--------|:------|:-----|
| DORN (ResNet)     | 2.271 | [Caffe](https://drive.google.com/file/d/1hQUsVmrh142fyoHVYnN5Ry6I3lXrEgAv) | [paper](http://openaccess.thecvf.com/content_cvpr_2018/CameraReady/3454.pdf) | [Caffe](https://github.com/hufu6371/DORN) |
| DORN (VGG)        | 2.517 | N/A | [paper](http://openaccess.thecvf.com/content_cvpr_2018/CameraReady/3454.pdf) | N/A |
| Kuznietsov et al. | 3.518 | [TensorFlow](https://www.vision.rwth-aachen.de/media/papers/best_model.tgz) | [paper](https://arxiv.org/abs/1702.02706) | [TensorFlow](https://github.com/Yevkuzn/semodepth) |


### KITTI < 80 m.

Max depth is restricted to 80 meters.

[Dataset description](datasets/kitti_depth_estimation.md)

| Model | Score | Weights | Paper | Code |
|:------|:-----:|:--------|:------|:-----|
| DORN (ResNet)     | 2.727 | [Caffe](https://drive.google.com/file/d/1hQUsVmrh142fyoHVYnN5Ry6I3lXrEgAv) | [paper](http://openaccess.thecvf.com/content_cvpr_2018/CameraReady/3454.pdf) | [Caffe](https://github.com/hufu6371/DORN) |
| DORN (VGG)        | 3.056 | N/A | [paper](http://openaccess.thecvf.com/content_cvpr_2018/CameraReady/3454.pdf) | N/A |
| Kuznietsov et al. | 4.621 | [TensorFlow](https://www.vision.rwth-aachen.de/media/papers/best_model.tgz) | [paper](https://arxiv.org/abs/1702.02706) | [TensorFlow](https://github.com/Yevkuzn/semodepth) |

### NYU Depth v2

[Dataset description](datasets/nyu_depth_v2.md)

| Model | Score | Weights | Paper | Code |
|:------|:-----:|:--------|:------|:-----|
| DORN (ResNet) | 0.509 | [Caffe](https://drive.google.com/file/d/1PkxkzWwZthjnJGtaPlTS5qTrj-Tka7eX/view) | [paper](http://openaccess.thecvf.com/content_cvpr_2018/CameraReady/3454.pdf) | [Caffe](https://github.com/hufu6371/DORN) |
| MS-CRF        | 0.586 | [Caffe](https://drive.google.com/drive/folders/0ByWGxNo3TouJRDFPdWF4UWFubVk) | [paper](https://arxiv.org/abs/1704.02157) | [Caffe](https://github.com/danxuhk/ContinuousCRF-CNN) |
| Li et al.     | 0.635 | N/A | [paper](https://arxiv.org/abs/1607.00730) | N/A |
