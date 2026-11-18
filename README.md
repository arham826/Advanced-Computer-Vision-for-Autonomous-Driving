# FSD Capstone Project

Self-driving car capstone: steering-angle prediction, lane segmentation and object detection.

## Dataset

The driving dataset (~45k images) is not included in this repo because of its size.

### Steering angle dataset

This is Sully Chen's driving dataset: 45,568 dashcam frames, each labelled with a steering angle.

- Download: https://github.com/SullyChen/driving-datasets

Extract it so the layout matches what `model_training/train_steering_angle/driving_data.py` expects:

```
data/
└── driving_dataset/
    ├── data.txt      # "<image>.jpg <steering angle>" per line
    ├── 0.jpg
    ├── 1.jpg
    └── ...
```

### Lane segmentation dataset

The lane segmentation notebook (`model_training/train_lame_detection/training_lane_deteciton.ipynb`) downloads its dataset from Roboflow. You need your own Roboflow API key, stored as `ROBOFLOW_API_KEY`.

- Roboflow project: https://universe.roboflow.com/aditya-choudhary-ehv9p/l-s-kvbur

## Setup

```bash
pip install -r requirements.txt
```
