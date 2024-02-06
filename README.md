**YOLOv8 Feature Extraction Repository:**
*Overview:*
While exploring the official YOLOv8 documentation available at [Ultralytics](https://www.ultralytics.com/), I faced a challenge in understanding the feature extraction process clearly. Although the documentation covers various aspects of YOLOv8 comprehensively, specific details regarding feature extraction appeared to be either lacking or unclear. In response to this, I have created this repository to fill the gap by providing a more explicit and accessible guide for feature extraction from YOLOv8. The code in this repository aims to offer a practical solution for users seeking to extract features from YOLOv8 (using the object detection model!) for their specific requirements.

**Dependencies**
Ensure you have the following dependencies installed before running the code:


pip install ultralytics
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
pip install numpy
Repository Contents
This repository contains code for feature extraction from YOLOv8, the latest version of the You Only Look Once (YOLO) object detection system. The implemented code efficiently extracts features from YOLOv8 and includes a plotting component to visualize these extracted features.

**How to Use ??**
Install the required dependencies by running the provided commands.
Navigate to the main code file and execute it to perform feature extraction.
Explore the generated plots to gain insights into the features extracted from YOLOv8.
Feel free to customize and extend the code based on your specific requirements. If you encounter any issues or have suggestions, please raise them in the repository's issue tracker.
YOLOv8 Performance
YOLOv8 demonstrates significant performance compared to the latest version and other object detection architectures. It has been investigated across various fields, including medical applications.

## Update on **YOLOv8** Architecture

An important update in this architecture is **YOLOv8's** reliance on three resolutions for feature extraction to classify and localize objects of interest:


| Resolution    | Object Size     |
| ------------- | --------------- |
| 80x80xdepth   | Smaller Object  |
| 40x40xdepth   | Medium Object   |
| 20x20xdepth   | Larger Object   |


| Layer | Resolution | Depth |
| ----- | ---------- | ----- |
| 13    | 80x80       | 256   |
| 14    | 80x80       | 384   |
| 15    | 80x80       | 128   |
| 16    | 40x40       | 128   |
| 17    | 40x40       | 384   |
| 18    | 40x40       | 256   |
| 19    | 20x20       | 256   |
| 20    | 20x20       | 768   |
| 21    | 20x20       | 512   |




