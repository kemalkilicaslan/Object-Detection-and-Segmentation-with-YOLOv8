# YOLOv8 Object Detection
## Installation
```
pip install ultralytics
```
___
### Image Detection
#### CLI (Command Line Interface)
```
yolo detect predict model=yolov8x.pt source="img.jpg" save=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
results = model('img.jpg', save=True)
```
**Example**

**Image**
![img](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Image.webp)

**Object Detection Image**
![Object-Detection-Image](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Detection-with-YOLOv8/Object-Detection-Image.webp)
___
### Video Detection
#### CLI (Comman Line Interface)
```
yolo detect predict model=yolov8x.pt source="video.mp4" save=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
results = model('video.mp4', save=True)
```
**Example**

**Video**
[![video](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Video.webp)](https://www.youtube.com/watch?v=wBG1KDi17QM)

**Object Detection Video**
[![Object-Detection-Video](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Detection-with-YOLOv8/Object-Detection-Video.webp)](https://www.youtube.com/watch?v=lvPSlkSZqyA)
___
### Live Detection
#### CLI (Command Line Interface)
```
yolo detect predict model=yolov8x.pt source=0 show=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
model.predict(source="0", show=True)
```
**Example**

**Real Time Object Detection**
[![Real-Time-Object-Detection](https://github.com/kemalkilicaslan/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Detection-with-YOLOv8/Real-Time-Object-Detection.webp)](https://www.youtube.com/watch?v=yvONGbaFJ0g)
