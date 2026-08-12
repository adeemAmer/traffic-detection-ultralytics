# Traffic Detection and Tracking using Ultralytics YOLO

## Project Overview

This project is a computer vision application for traffic analysis using Ultralytics YOLO.

The system performs:
- Object detection on traffic images and videos.
- Object tracking with unique object IDs.
- Model evaluation using mAP50, mAP50-95, Precision, and Recall.
- Custom training for car detection.
- Model export to ONNX format.

## Technologies

- Python
- Ultralytics YOLO
- Google Colab
- OpenCV
- ONNX

## Model Evaluation

The trained model was evaluated using `model.val()`.

| Metric | Result |
|---|---:|
| mAP50 | 0.5186 |
| mAP50-95 | 0.3681 |
| Precision | 0.6334 |
| Recall | 0.4748 |

These metrics provide an overall indication of the model's detection performance. Precision measures how many predicted detections were correct, while Recall measures how many relevant objects were detected.

## Custom Training

A custom car dataset was prepared from a traffic image using automatically generated YOLO labels.

The custom training was performed using:

- Epochs: 5
- Image size: 640
- Batch size: 1
- Class: car

The trained custom model was saved as:

`custom_car_best.pt`

## Tracking

The project applies YOLO tracking to traffic video and assigns IDs to detected objects.


## Project Files

- `Untitled FINAL.ipynb` - Main project notebook.
- `custom_car_best.pt` - Custom trained car detection model.
- `TRACKING_FINAL_H264.mp4` - Final traffic detection and tracking video.

## Training Program

This project was completed as part of:

**Computer Vision for Developers with Ultralytics**

Delivered by **SDAIA Academy** through Learning Space.

SDAIA Academy:
https://github.com/SDAIAAcademy
## Demo Video
The final tracking video can be viewed by clicking *View raw* on the video file.
[▶️ View Final Tracking Video](./TRACKING_FINAL_H264.mp4)
