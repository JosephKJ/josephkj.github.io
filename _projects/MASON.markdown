---
layout: page
title: 'MASON: A Model AgnoStic ObjectNess Framework'
description: European Conference on Computer Vision, Workshop Proceedings (ECCV-W), Munich, Germany. 2018
comments: true
# img: /assets/img/12.jpg
---

#### Prologue

MASON proposes a simple, yet very effective method to localize dominant foreground objects
in an image, to  pixel-level precision. The proposed method `MASON' (Model-AgnoStic ObjectNess)
uses a deep convolutional network to generate category-independent and model-agnostic
heat maps for any image. The network is not explicitly trained for the task and hence,
can be used off-the-shelf in tandem with any other network or task.
We show that this framework scales to a wide variety of images,
and illustrate the effectiveness of MASON in three varied application contexts.

#### Task 1: Foreground Segmentation
<img class="col three" src="{{ site.baseurl }}/assets/img/mason/foreground_seg.png" alt="" title="example image"/>
The effectiveness of MASON in fine-grained object localization is captured in the figure (Column 3). The proposed method (Column 3) is more effective than just using Grabcut (Column 4) in foreground segmentation.

#### Task 2: Extending object detectors to perform instance segmentations
<iframe width="560" height="315" src="https://www.youtube.com/embed/GG_Pr8hdZhY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
<iframe width="560" height="315" src="https://www.youtube.com/embed/VjSRRxCoHTI" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

#### Task 3: Improving the quality of detection datasets
<img class="col three" src="{{ site.baseurl }}/assets/img/mason/cleaning.png" alt="" title="example image"/>
The picture captures the effectiveness of \method to enhance bad annotations in a dataset. False positive annotations are removed and remaining annotations are made tighter by MASON. The image is the 4005th frame from Video 0 of `Bookstore' scene in the Stanford Drone Dataset. Red color bounding boxes annotate Pedestrians while blue color annotate Biker.


#### Code

Code for MASON: [https://github.com/JosephKJ/MASON](https://github.com/JosephKJ/MASON)