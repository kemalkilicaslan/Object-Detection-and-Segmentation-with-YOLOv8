# YOLOv8 Object Segmentation
## Installation
```
pip install ultralytics
```
___
### Image Segmentation
#### CLI (Command Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='img.jpg' save=true
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
results = model('img.jpg', save=True)
```
**Example**

**Image**
![img](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Image.webp)

**Object Segmentation Image**
![Object-Segmentation-Image](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Segmentation-with-YOLOv8/Object-Segmentation-Image.webp)
___
### Video Segmentation
#### CLI (Comman Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='video.mp4' save=true
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
results = model('video.mp4', save=True)
```
**Example**

**Video**
[![video](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Video.webp)](https://www.youtube.com/watch?v=wBG1KDi17QM)

**Object Segmentation Video**
[![Object-Segmentation-Video](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Segmentation-with-YOLOv8/Object-Segmentation-Video.webp)](https://www.youtube.com/watch?v=psdXMi5fQ8U)
___
### Live Segmentation
#### CLI (Command Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='0' show=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
model.predict(source="0", show=True)
```
**Example**

**Real Time Object Segmentation**
[![Real-Time-Object-Segmentation](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Segmentation-with-YOLOv8/Real-Time-Object-Segmentation.webp)](https://www.youtube.com/watch?v=bhdDW9Fkcw0)
