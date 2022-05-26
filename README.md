# CS230_DAA
Code for CS230 course project on implementing a vision-based detect and avoid (DAA) system.

![](https://github.com/smkatz12/CS230_DAA/blob/main/results/test_above.gif)

### Getting set up with X-Plane 11
The data generation files in this repository require [X-Plane 11](https://www.x-plane.com) and the [XPlaneConnect Plugin](https://github.com/nasa/XPlaneConnect). Information about how to set this up can be found [here](https://github.com/StanfordASL/NASA_ULI_Xplane_Simulator).

### File Overview
`src/data_generation/generate_traffic_data_py`: script to generate images of intruder aircraft at various relative positions and save to a specified folder

`src/data_generation/label_traffic_data.py`: script to generate bounding box labels for a set of images given the relative position of the intruder aircraft

`src/data_generation/tune_bounding.ipynb`: notebook used to tune parameters for bounding box labeling

`src/data_generation/xpc3.py`: code required to interface with X-Plane 11

`src/yolo_v5/`: code to train yolo network (see [here](https://github.com/ultralytics/yolov5))

`src/util.py`: utility functions for loading in networks and evaluating them on images from X-Plane 11

`src/CS230_results.ipynb`: notebook with results analysis and figure generation code

`models/`: contains models for three trials

`results/`: gifs of results