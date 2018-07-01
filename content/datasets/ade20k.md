# ADE20K

### Description

* [Scene Parsing through ADE20K Dataset](http://people.csail.mit.edu/bzhou/publication/scene-parse-camera-ready.pdf)
* [Semantic Understanding of Scenes through ADE20K Dataset](https://arxiv.org/pdf/1608.05442.pdf)
* [Official website](http://groups.csail.mit.edu/vision/datasets/ADE20K/)

Challenges using ADE20K data:

* [MIT Scene Parsing Benchmark (2016)](http://sceneparsing.csail.mit.edu/)
* [Places Challenge (ICCV 2017)](http://placeschallenge.csail.mit.edu/)

Evaluation is usually done in the framework of competitions.
For the target metric in both Scene Parsing and Places the authors use
the average of Pixel Accuracy and Mean Intersection over Union.


### Downloads

#### Original ADE20K

* [Full dataset (3.8G .zip)](http://groups.csail.mit.edu/vision/datasets/ADE20K/ADE20K_2016_07_26.zip)

#### MIT Scene Parsing Challenge

The data comes from original ADE20K dataset

* [Train/Val](http://data.csail.mit.edu/places/ADEchallenge/ADEChallengeData2016.zip)
* [Test Set](http://data.csail.mit.edu/places/ADEchallenge/release_test.zip)


### Technical details

* 20 210 images in **training set**, 2000 images in **validation set**, 3000 images in **testing set**.
* 20 object classes and 434 826 object instances.
* Finer hierarchical labeling beyond 20 object classes: 150 stuff/object labels (e.g. wall, sky, tree)
and 1038 image-level labels (e.g. airport terminal, bedroom, street)
* Varying spatial resolution: median image size - 307 200 pixels with median aspect ratio of 1.33.

### Format

Each folder contains images separated by scene category (same scene categories than the Places Database). For each image, the object and part segmentations are stored in two different png files. All object and part instances are annotated sparately.

For each image there are the following files:

##### \*.jpg

Input RGB image.

##### \*_seg.png

RGB image with object segmentation mask. The mask has the following structure:

##### \*_seg_parts_N.png

Parts segmentation mask, where N is a number (1,2,3,...) indicating the level in the part hierarchy.
N=1 - parts of objects. As N can be > 1, parts can consist of parts too.

##### \*_.txt

Text file describing the content of each image (describing objects and parts).
This information is redundant with other files. But in addition contains also information about object attributes.
The function `loadAde20K.m` provided in official toolkit (see below) also parses the content of this file.
Each line in the text file contains six columns with the following content:

1. Instance number
2. Part level (0 for objects),
3. Indicator of occlusion (1 for true)
4. Class name (parsed using wordnet)
5. Original raw name (might provide a more detailed categorization)
6. Comma separated attributes list

### Resources

| Link | Description |
|:-----|:------------|
| [Segmentation models for ADE20K (PyTorch)](https://github.com/CSAILVision/semantic-segmentation-pytorch) | PyTorch implementation of segmentation models and training routines |
| [MATLAB Development Kit](https://github.com/CSAILVision/sceneparsing)| Evaluation/Visualization scripts |
| [Baselines from MIT Team](https://github.com/CSAILVision/sceneparsing/wiki/Model-Zoo) | A bunch of pretrained PyTorch models |
| [Official MATLAB tools for loading](http://groups.csail.mit.edu/vision/datasets/ADE20K/code.zip) | MATLAB scripts for loading and exploring the data |

### Demo

A sample of images (row 1) with corresponding object-level (row 2) and parts-level (row 3) segmentations:

[Hi-res sample](http://groups.csail.mit.edu/vision/datasets/ADE20K/assets/images/examples.png)

A web-based tool for browsing different data splits:

* [Training set](http://sceneparsing.csail.mit.edu/browse.php/?dirname=training/)
* [Validation set](http://sceneparsing.csail.mit.edu/browse.php/?dirname=validation/)