# Face Mask Detection - YOLOv5

## What is YOLOv5 ?
YOLOv5 rocket is a family of object detection architectures and models pretrained on the COCO dataset, and represents Ultralytics open-source research into future vision AI methods, incorporating lessons learned and best practices evolved over thousands of hours of research and development.

## What Face Mask Detection Do ?
Face mask detection refers to detect whether a person is wearing a mask or not. In fact, the problem is reverse engineering of face detection where the face is detected using different machine learning algorithms for the purpose of security, authentication and surveillance.

## How to use ?
### 1. Environment Setup
clone this GitHub repository

    git clone https://github.com/rohitrrg/Face_Mask_Detection-YOLOv5.git

go inside the project directory

    cd Face_Mask_Detection-YOLOv5

install necessary packages

    pip install -r requirements.txt

### 2. Run Inference
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

![South-Korea-introduces-mask-mandate-in-COVID-19-fight](https://user-images.githubusercontent.com/43450375/219920117-b48fee9d-2659-4e99-ac24-dae786c2d44e.jpg)

You can also Detect any specific class like only faces which are not wearing or incorrectly wearing masks in the crowd.

    python detect.py --weights best.pt --source img.jpg --classes 1 2

![South-Korea-introduces-mask-mandate-in-COVID-19-fight](https://user-images.githubusercontent.com/43450375/219920220-3c82cc24-140e-4389-a8ac-f398d2464d3f.jpg)

Other arguments

    --weights	   	    'model path or triton URL'
    --source		    'file/dir/URL/glob/screen/0(webcam)'
    --data 			    (optional) dataset.yaml path'
    --img'			    'inference size h,w'
    --conf-thres	    'confidence threshold'
    --iou-thres		    'NMS IoU threshold'
    --max-det		    'maximum detections per image'
    --device		    'cuda device, i.e. 0 or 0,1,2,3 or cpu'
    --view-img		    'show results'
    --save-txt		    'save results to *.txt'
    --save-conf		    'save confidences in --save-txt labels'
    --save-crop		    'save cropped prediction boxes'
    --nosave		    'do not save images/videos'
    --classes		    'filter by class: --classes 0, or --classes 0 2 3'
    --agnostic-nms	    'class-agnostic NMS'
    --augment		    'augmented inference'
    --visualize		    'visualize features'
    --update		    'update all models'
    --project		    'save results to project/name'
    --name			    'save results to project/name'
    --exist-ok		    'existing project/name ok, do not increment'
    --line-thickness    'bounding box thickness (pixels)'
    --hide-labels		'hide labels'
    --hide-conf		    'hide confidences'
    --half			    'use FP16 half-precision inference'
    --dnn			    'use OpenCV DNN for ONNX inference'
    --vid-stride		'video frame-rate stride'
