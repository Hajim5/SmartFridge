# SmartFridge: Intelligent Recipe Recommendation System

## Overview
The SmartFridge project uses YOLOv5 and a custom dataset to detect items in a fridge and recommend recipes based on the detected ingredients. This system integrates object detection, recipe matching, and a user-friendly interface to enhance the cooking experience.

---

## Features
- **Food Item Detection:** High-accuracy detection of food items inside the fridge using YOLOv5 and a custom dataset.
- **Recipe Recommendation:** Suggests recipes based on available ingredients.
- **Dynamic Database Integration:** JSON-based recipe database for easy expansion.
- **Custom Training:** Training the YOLOv5 model on a custom dataset using Google Colab.
- **Roboflow Integration:** Efficient dataset annotation and management via the Roboflow API.

---

## Dataset and Model
The dataset and model are hosted on Roboflow. You can access them [here](https://universe.roboflow.com/capstoneproject-yly17/fridge_roboflow/model/1).

### **Example: Download Dataset via API**
```python
from roboflow import Roboflow

rf = Roboflow(api_key="YOUR_API_KEY")
project = rf.workspace().project("fridge_roboflow")
dataset = project.version(1).download("yolov5")

### Demo
Here's an example of the SmartFridge system in action:

**Step 1: Object Detection in the Fridge**
![Object Detection](path/to/center_shelf_demo_result.jpg)

**Step 2: Recipe Recommendation Based on Detected Ingredients**
![Recipe Recommendation](path/to/screenshot2.png)

