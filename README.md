# face_detection_caffe
This is an implementation of "Towards a Deep Learning Framework for Unconstrained Face Detection " (arxiv 2016) in caffe.

We train with wider face dataset + vgg16 network pre-training + faster rcnn + multi scale 
 represention + l2 normalize + scale, more information you can refer to above paper.
### Introduction
This repository is a fork from [py-faster-rcnn](https://github.com/rbgirshick/py-faster-rcnn).
You can refer to [py-faster-rcnn README.md](https://github.com/rbgirshick/py-faster-rcnn/blob/master/README.md) and [faster-rcnn README.md](https://github.com/ShaoqingRen/faster_rcnn/blob/master/README.md) for more information.
##Setup
1.put wider_face.py and fddb.py in lib/datasets/ 

2.put train_ms.prototxt, test_ms.prototxt, slover_ms.prototxt in models/wider_face/VGG16/faster_rcnn_end2end/

3.put faster_rcnn_end2end_ms.sh in experiments/scripts/

4.put normalize_layer.cpp normalize_layer.cu normalize_layer.hpp in your caffe dir

and other steps are same as py-faster-rcnn
