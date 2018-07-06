# Object detection

## Description

The problems is formulated as predicting a bounding box with corresponding class label
for each object in the input image. Each image can contain several objects.

Two main metrics are mean Average Precision (mAP) and mean Average Recall (mAR).
For additional information on competition-specific metrics please refer to the dataset descriptions.

## Results

### MS-COCO 2016

[Dataset description](datasets/coco_detection.md)

Results taken from [Google Research Model Zoo](https://github.com/tensorflow/models/tree/master/research/object_detection)

In addition to mAP for each model we include inference time in milliseconds per image on frozen inference graphs.

| Model | mAP, % | Inference time, ms | Weights | Paper | Code |
|:------|:-----:|:-----:|:--------|:------|:-----|
| Faster R-CNN NasNet              | 43 | 1833 | [TensorFlow](http://download.tensorflow.org/models/object_detection/faster_rcnn_nas_coco_2018_01_28.tar.gz) | [paper](https://arxiv.org/abs/1506.01497) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/faster_rcnn_meta_arch.py) |
| Faster R-CNN Inception-ResNet-v2 | 37 | 771  | [TensorFlow](http://download.tensorflow.org/models/object_detection/mask_rcnn_inception_resnet_v2_atrous_coco_2018_01_28.tar.gz) | [paper](https://arxiv.org/abs/1506.01497) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/faster_rcnn_meta_arch.py) |
| Faster R-CNN ResNet-101          | 32 | 470  | [TensorFlow](http://download.tensorflow.org/models/object_detection/faster_rcnn_resnet101_coco_2018_01_28.tar.gz) | [paper](https://arxiv.org/abs/1506.01497) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/faster_rcnn_meta_arch.py) |
| Faster R-CNN ResNet-50           | 30 | 343  | [TensorFlow](http://download.tensorflow.org/models/object_detection/faster_rcnn_resnet50_coco_2018_01_28.tar.gz) | [paper](https://arxiv.org/abs/1506.01497) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/faster_rcnn_meta_arch.py) |
| R-FCN ResNet-101                 | 30 | 92   | [TensorFlow](http://download.tensorflow.org/models/object_detection/rfcn_resnet101_coco_2018_01_28.tar.gz) | [paper](https://arxiv.org/abs/1605.06409) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/rfcn_meta_arch.py) |
| Faster R-CNN Inception-v2        | 28 | 58   | [TensorFlow](http://download.tensorflow.org/models/object_detection/faster_rcnn_inception_v2_coco_2018_01_28.tar.gz) | [paper](https://arxiv.org/abs/1506.01497) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/faster_rcnn_meta_arch.py) |
| SSD Inception-v2                 | 24 | 42   | [TensorFlow](http://download.tensorflow.org/models/object_detection/ssd_inception_v2_coco_2018_01_28.tar.gz) | [paper](https://arxiv.org/abs/1512.02325) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/ssd_meta_arch.py) |
| SSD MobileNet-v2                 | 22 | 31   | [TensorFlow](http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v2_coco_2018_03_29.tar.gz) | [paper](https://arxiv.org/abs/1512.02325) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/ssd_meta_arch.py) |
| SSD-Lite MobileNet-v2            | 22 | 27   | [TensorFlow](http://download.tensorflow.org/models/object_detection/ssdlite_mobilenet_v2_coco_2018_05_09.tar.gz) | [paper](https://arxiv.org/abs/1512.02325) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/ssd_meta_arch.py) |
| SSD MobileNet-v1                 | 21 | 30   | [TensorFlow](http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v1_coco_2018_01_28.tar.gz) | [paper](https://arxiv.org/abs/1512.02325) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/object_detection/meta_architectures/ssd_meta_arch.py) |

## Resources

| Title | Type | Description |
|:------|:----:|:------------|
| [Supercharge your Computer Vision models with the TensorFlow Object Detection API](https://ai.googleblog.com/2017/06/supercharge-your-computer-vision-models.html) | Post | Announcement of open-source object detection models releaseby Google Research |