# Automatic-scene-segmentation-in-movies
## Introduction
With applications in the entertainment sector including scene retrieval and video editing, movie scene segmentation is a difficult computer vision problem. A scene is made up of one or more shots that are connected in terms of time, place, and theme. A shot is a continuous series of images, whereas a scene is a higher-level semantic unit. Although there has been a lot of research on scene boundary detection in videos, there is still room for improvement. Scene boundary detection methods such as shot contrastive learning and supervised classification have recently been proposed, but they have drawbacks. In this study, the we suggest tackling the issue of movie scene recognition by replacing sub-problems with cutting-edge models to enhance the precision and effectiveness of current deep-learning models. 
## Running the Code 
### Data Collection
To run the code, you need to download the movienet dataset from https://opendatalab.com/MovieNet/download, and also labels from https://drive.google.com/drive/folders/1w_qdnRsxF1w1rMuMbdCe1JLHeZ0MZ6A8 
### Running
Run feature_extraction_movienet_tools.ipynb to extract place, person and face feature from frames of shots

feature_visualization.ipynb shows similarity score of different features for a sequence of frames

model_final.ipynb and model_cnn.ipynb contains dataloader,training as well as testing code, which can be ran to obatin average precision scores

## Results
Without LSTM :
AP: 0.327
With LSTM :
AP : 0.347
<img width="167" alt="image" src="https://user-images.githubusercontent.com/60317512/236277098-b49e0eaf-3c13-4eb6-a717-5cefde5e27ee.png">

<img width="161" alt="image" src="https://user-images.githubusercontent.com/60317512/236276811-5942abaf-40c9-4140-81ee-2d94284d1ee3.png">

## References
@inproceedings{rao2020local,
title={A Local-to-Global Approach to Multi-modal Movie Scene Segmentation},
author={Rao, Anyi and Xu, Linning and Xiong, Yu and Xu, Guodong and Huang, Qingqiu and Zhou, Bolei and Lin, Dahua},
booktitle={IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
year={2020}
}

https://github.com/AnyiRao/SceneSeg

https://github.com/movienet
