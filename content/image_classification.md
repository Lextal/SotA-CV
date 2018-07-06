# Image classification

## Description

Assigning a single class label to the whole input image.

Metrics:
* Top-1 Accuracy
* Top-5 Accuracy

## Results

### ImageNet

Single model, single crop. Top-5 results by Acc@5 are highlighted in boldface as well.

[Dataset description](datasets/imagenet_classification.md)


| Model               |  Acc@1 |  Acc@5 | Weights | Paper | Code |
|:--------------------|:------:|:------:|:--------|:------|:-----|
| DenseNet-121        | **82.858** | 92.290 | [PyTorch](https://download.pytorch.org/models/densenet121-a639ec97.pt) | [paper](https://arxiv.org/abs/1608.06993) | [PyTorch](https://github.com/pytorch/vision/blob/master/torchvision/models/densenet.py) |
| DenseNet-161        | **82.736** | 93.798 | [PyTorch](https://download.pytorch.org/models/densenet161-8d451a50.pth) | [paper](https://arxiv.org/abs/1608.06993) | [PyTorch](https://github.com/pytorch/vision/blob/master/torchvision/models/densenet.py) |
| DenseNet-169        | **82.693** | 93.150 | [PyTorch](https://download.pytorch.org/models/densenet169-b2777c0a.pth) | [paper](https://arxiv.org/abs/1608.06993) | [PyTorch](https://github.com/pytorch/vision/blob/master/torchvision/models/densenet.py) |
| DenseNet-201        | **82.566** | 93.660 | [PyTorch](https://download.pytorch.org/models/densenet201-c1103571.pth) | [paper](https://arxiv.org/abs/1608.06993) | [PyTorch](https://github.com/pytorch/vision/blob/master/torchvision/models/densenet.py) |
| Inception-v1        | **81.320** | 89.600 | [TensorFlow](http://download.tensorflow.org/models/inception_v1_2016_08_28.tar.gz) | [paper](http://arxiv.org/abs/1409.4842v1) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v1.py) |
| Inception-v2        | 81.304 | 91.800 | [TensorFlow](http://download.tensorflow.org/models/inception_v2_2016_08_28.tar.gz) | [paper](http://arxiv.org/abs/1502.03167) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v2.py) |
| Inception-v3        | 80.400 | 93.900 | [TensorFlow](http://download.tensorflow.org/models/inception_v3_2016_08_28.tar.gz) [PyTorch](https://download.pytorch.org/models/inception_v3_google-1a9a5a14.pth) | [paper](http://arxiv.org/abs/1502.03167) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v3.py) [PyTorch](https://github.com/pytorch/vision/blob/master/torchvision/models/inception.py) |
| Inception-v4        | 80.200 | 95.200 | [TensorFlow](http://download.tensorflow.org/models/inception_v4_2016_09_09.tar.gz) | [paper](http://arxiv.org/abs/1602.07261) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v4.py) |
| Inception-v4        | 80.170 | 94.930 | [PyTorch](http://data.lip6.fr/cadene/pretrainedmodels/inceptionv4-8e4777a0.pth) | [paper](http://arxiv.org/abs/1602.07261) | [PyTorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/inceptionv4.py) |
| Inception-ResNet-v2 | 80.060 | **95.300** | [TensorFlow](http://download.tensorflow.org/models/inception_resnet_v2_2016_08_30.tar.gz) | [paper](http://arxiv.org/abs/1602.07261) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_resnet_v2.py) |
| Inception-ResNet-v2 | 78.888 | **95.234** | [PyTorch](http://data.lip6.fr/cadene/pretrainedmodels/inceptionresnetv2-520b38e4.pth) | [paper](http://arxiv.org/abs/1602.07261) | [PyTorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/inceptionresnetv2.py) |
| NASNet-A-Large      | 78.428 | **96.163** | [TensorFlow](https://storage.googleapis.com/download.tensorflow.org/models/nasnet-a_large_04_10_2017.tar.gz) | [paper](https://arxiv.org/abs/1707.07012) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/slim/nets/nasnet/nasnet.py) |
| NASNet-A-Large      | 78.000 | **96.086** | [PyTorch](http://data.lip6.fr/cadene/pretrainedmodels/nasnetalarge-a1897284.pth) | [paper](https://arxiv.org/abs/1707.07012) | [PyTorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/nasnet.py) |
| PNASNet-5-Large     | 77.560 | **96.182** | [TensorFlow](https://storage.googleapis.com/download.tensorflow.org/models/pnasnet-5_large_2017_12_13.tar.gz) | [paper](https://arxiv.org/abs/1712.00559) | [TensorFlow](https://github.com/tensorflow/models/blob/master/research/slim/nets/nasnet/pnasnet.py) |
| PNASNet-5-Large     | 77.438 | 95.992 | [PyTorch](http://data.lip6.fr/cadene/pretrainedmodels/pnasnet5large-bf079911.pth) | [paper](https://arxiv.org/abs/1712.00559) | [PyTorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/pnasnet.py) |
| SENet154            | 77.420 | 95.530 | [Caffe](https://drive.google.com/file/d/0BwHV3BlNKkWlbTFZbzFTSXBUTUE/view?usp=sharing) | [paper](https://arxiv.org/abs/1709.01507) | [Caffe](https://github.com/hujie-frank/SENet) |
| FBResNet-152        | 77.386 | 93.594 | [PyTorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/fbresnet.py) | [paper](https://arxiv.org/abs/1512.03385) | [PyTorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/fbresnet.py) |
| SENet154            | 76.200 | 95.498 | [PyTorch](http://data.lip6.fr/cadene/pretrainedmodels/senet154-c7b49a05.pth) | [paper](https://arxiv.org/abs/1709.01507) | [PyTorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/senet.py) |
| Xception            | 74.980 | 94.292 | [PyTorch](http://data.lip6.fr/cadene/pretrainedmodels/xception-b5690688.pth) | [paper](https://arxiv.org/abs/1610.02357) | [PyTorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/xception.py) |
| ResNet-101          | 73.900 | 93.672 | [PyTorch](https://download.pytorch.org/models/resnet101-5d3b4d8f.pth) | [paper](https://arxiv.org/abs/1512.03385) | [PyTorch](https://github.com/pytorch/vision/blob/master/torchvision/models/resnet.py) |





### PASCAL VOC Classification

TODO: add dataset description

[Dataset description](datasets/...)

| Model | Score | Weights | Paper | Code |
|:------|:-----:|:--------|:------|:-----|
| Model name | 0.5 | [link to the weights of a trained model]() | [paper](https://arxiv.org/abs/0000.00000) | [link to implementation]() |

## Resources


| Title | Type | Description |
|:------|:----:|:------------|
| [pretrained-models.pytorch](https://github.com/Cadene/pretrained-models.pytorch) | Repository | Repo dedicated to reproduction of research paper results and collect pretrained convolutional nets for classification (PyTorch). |
| [tf/research/slim](https://github.com/tensorflow/models/tree/master/research/slim) | Repository | Convolutional nets for classification pretrained on ImageNet (TF Slim) |
