The processed Charades Captions are stored in the json file `charades_captions.json` as a list. 
Each entry in the list is a video dictionary, which contains:

- id:
Unique identifier for each video.
- captions:
Multiple captions that describe the video.
- seg_labels:
Binary segment labels for every token. 1 means the corresponding token is the end of the segment.
- scene:
One of 15 indoor scenes in the dataset, such as Kitchen
- actions:  
Semicolon-separated list of "class start end" triplets for each actions in the video, such as c092 11.90 21.20;c147 0.00 12.60
- length:
The length of the video in seconds
- path:
The path to the video directory in your local machine. Can be changed as you wish.
- split:
Which set the video belongs to. `train`, `validate` or `test`.


For more details, please refer to:
1. Our paper: Video Captioning via Hierarchical Reinforcement Learning (https://arxiv.org/abs/1711.11135)
2. Original Charades dataset: http://allenai.org/plato/charades/ 


If this dataset helps your research, please cite:

@article{wang2018video,
title={Video Captioning via Hierarchical Reinforcement Learning},
author={Wang, Xin and Chen, Wenhu and Wu, Jiawei and Wang, Yuan-Fang and Wang, William Yang},
journal={CVPR},
year={2018}
}