# Plants-Disease-Detection
An AI Model built with Yollov11 , Trained to Detect 9 Plants Diseases (90.7%)Acc
---
language: en
tags:
- yolo
- object-detection
- computer-vision
datasets:
- https://universe.roboflow.com/learning-eri4b/plant-disease-tmyq8
---

# YOLO Object Detection Model

This model is trained to detect Detect 9 Plants Diseases .

## Model Details

- Model Type: YOLOv11 
- Training Dataset: [Dataset information]
- Performance Metrics: [90.7]
- Classes: [bercak_daun ,daun_okra ,daun_strawberry ,daun_tomat ,defisiensi_kalsium ,hangus_daun ,hawar_daun ,mosaik_vena_kuning ,virus_kuning_keriting]
## Usage

```python
from ultralytics import YOLO
from huggingface_hub import hf_hub_download

# Download the model
model_path = hf_hub_download(repo_id="your-username/your-model-name", filename="best.pt")

# Load the model
model = YOLO(model_path)

# Make predictions
results = model("path/to/image.jpg")
