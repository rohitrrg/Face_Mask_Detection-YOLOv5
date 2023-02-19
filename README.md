# Face Mask Detection - YOLOv5

## What is YOLOv5 ?
YOLOv5 rocket is a family of object detection architectures and models pretrained on the COCO dataset, and represents Ultralytics open-source research into future vision AI methods, incorporating lessons learned and best practices evolved over thousands of hours of research and development.

## What Face Mask Detection Do ?
Face mask detection refers to detect whether a person is wearing a mask or not. In fact, the problem is reverse engineering of face detection where the face is detected using different machine learning algorithms for the purpose of security, authentication and surveillance.

## How to use ?
## 1. Environment Setup
clone this GitHub repository

    git clone https://github.com/rohitrrg/Face_Mask_Detection-YOLOv5.git

go inside the project directory

    cd Face_Mask_Detection-YOLOv5

install necessary packages

    pip install -r requirements.txt

## 2. Run Inference
You can run YOLOv5 detection inference on images, videos, directories, globs, YouTube, webcam, streams, etc.

  
    python detect.py --weights best.pt --source 0                               # webcam
                                                     img.jpg                         # image
                                                     vid.mp4                         # video
                                                     screen                          # screenshot
                                                     path/                           # directory
                                                     list.txt                        # list of images
                                                     list.streams                    # list of streams
                                                     'path/*.jpg'                    # glob
                                                     'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                                                     'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream


