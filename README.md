# KBVQA - Knowledge-based Reasoning for Visual Question Answering

***Phase 2:***

**The progress and demo for phase 2 is documented in KBVQA_Demo.ipynb**


***Phase 1:***

In this project we are trying to analyze and improve on Explicit Knowledge-based Reasoning for Visual Question Answering(KBVQA).  
The files in the project have been modified from Hierarchical Question-Image Co-Attention for Visual Question Answering: 

https://github.com/jiasenlu/HieCoAttenVQA 

We tried to implement this VQA model but **it didn't work**. The details of this model are given below: 


*The folders in the repository contain code files for the following purposes:*  
The **data** folder contains code to download the dataset including: VQA data and COCO-QA dataset.
For the VQA dataset, the training, test and validation sets are downloaded from:

https://s3.amazonaws.com/cvmlp/vqa/mscoco/vqa/Questions_Train_mscoco.zip

https://s3.amazonaws.com/cvmlp/vqa/mscoco/vqa/Questions_Val_mscoco.zip

https://s3.amazonaws.com/cvmlp/vqa/mscoco/vqa/Questions_Test_mscoco.zip 

The VQA annotations are downloded from:

https://s3.amazonaws.com/cvmlp/vqa/mscoco/vqa/Annotations_Train_mscoco.zip

https://s3.amazonaws.com/cvmlp/vqa/mscoco/vqa/Annotations_Val_mscoco.zip

The COCO-QA data is downloaded from:

http://www.cs.toronto.edu/~mren/imageqa/data/cocoqa/cocoqa-2015-05-17.zip

The preprocessing of the VQA data is performed using **vqa_preprocess.py**  
The preprocessing of the COCO-QA data is performed using **cocoqa_preprocess.py**

The **image_model** folder contains code to download the models: VGG_ILSVRC_19_layers model and Deep Residual network implement by Facebook model  
The VGG model is downloaded from:  

http://www.robots.ox.ac.uk/~vgg/software/very_deep/caffe/VGG_ILSVRC_19_layers.caffemodel

The Deep Residual model is downloaded from:  

https://d2j0dndfm35trm.cloudfront.net/resnet-200.t7

The image models are downloaded using **download_model.py**

The **prepro** folder contains code to generate Image/Question features for VQA and COCO-QA.  
The files used for acheiving this are **prepro_vqa.py** and **prepro_cocoqa.py**

To extract the VGG image feature **repro_img_vgg.lua** is used.

**train.lua** is used to train the VQA and COCO-QA model.

