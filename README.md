# YOLO-Object-detection
In this repo you will learn how to use yolo object detection on images and realtime videos also.YOLO is a pretty trained model for u to predict a huge no of objects.There are several versions of yolo,like the yolo v3 which is used for detecting.
# REQUIREMENTS:
 download the yolov3 weights with their classes put them in the folder of yolo-coco
# MODULES USED:
  pip install numpy
  pip install argparse
  pip install opencv-python
  pip install imutils
 # instructions:
  $ tree 
  .
  ├── images
  │   ├── sample.jpg      //These are input image files
  │   ├── dining_table.jpg
  │   ├── living_room.jpg
  │   └── soccer.jpg
  ├── output
  │   ├── airport_output.avi
  │   ├── car_chase_01_output.avi       //These are the processed YoLo output video files
  │   ├── car_chase_02_output.avi
  │   └── overpass_output.avi
  ├── videos
  │   ├── airport.mp4
  │   ├── car_chase_01.mp4             // These are the input video files for processing
  │   ├── car_chase_02.mp4
  │   └── overpass.mp4
  ├── yolo-coco
  │   ├── coco.names                    //These files are mandatory for YoLo operations
  │   ├── yolov3.cfg                    //https://pjreddie.com/media/files/yolov2-tiny.weights     
  │   └── yolov3.weights                //https://github.com/pjreddie/darknet/blob/master/cfg/yolov2-tiny.cfg
  ├── yolo.py
  └── yolo_video.py

After downloading the weights files and cfg files , rename them according to tree structure 
For example , the downloaded file is "yolov2-tiny.weights" ==>> "yolov3.weights"
Similarly , for "yolov2-tiny.cfg"  ===>>  "yolov3.cfg"

Note that the rename process is very important ,orelse the program won't run.

To run the program  goto to terminal and type the following
1. To process the image file, enter the following
	python yolo.py --image images/sample.jpg --yolo yolo-coco
2.To process the video file , enter the following
	python yolo_video.py --input video/yourvideo.mp4 --output output/output.avi --yolo yolo-coco
