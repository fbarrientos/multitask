# Joint Object Detection and Semantic Segmentation
## Overview
Model based on CNNs that integrates object detection and semantic segmentation in lentic water scenes to simultaneously identify and localize navigational obstacles and amorphous semantic structures such as cyanobacterial blooms, water bodies, among others.

<img src="data/githubimage/000001.jpg">

## Setup
1. Clone this repository: `!git clone https://github.com/fbarrientos/multitask`
2. `%cd multitask`
3. Install libraries: `!python -m pip install -r requirements.txt`

## Train
`!python train_custom.py --data ./data/custom.yaml --cfg ./models/yolov5s_custom_seg.yaml --batch-size 16 --epochs 100 --weights ./yolov5s.pt --workers 8 --label-smoothing 0.1 --img-size 832 --noautoanchor --device 0`

