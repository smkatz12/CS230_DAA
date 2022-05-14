# CS230_DAA
Code for CS230 course project on implementing a vision-based detect and avoid (DAA) system.

### Getting set up with X-Plane 11
The data generation files in this repository require [X-Plane 11](https://www.x-plane.com) and the [XPlaneConnect Plugin](https://github.com/nasa/XPlaneConnect). Information about how to set this up can be found [here](https://github.com/StanfordASL/NASA_ULI_Xplane_Simulator).

### File Overview
`src/data_generation/generate_traffic_data_py`: script to generate images of intruder aircraft at various relative positions and save to a specified folder

`src/data_generation/label_traffic_data.py`: script to generate bounding box labels for a set of images given the relative position of the intruder aircraft

`src/data_generation/tune_bounding.ipynb`: notebook used to tune parameters for bounding box labeling

`src/yolo_v5/`: code to train yolo network (see [here](https://github.com/ultralytics/yolov5))

`models/uniform_v1`: baseline model

`results/`: gifs of preliminary results