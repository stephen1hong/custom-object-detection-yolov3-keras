# single-object-detection-yolov3-keras

* Setting

 ** python 3.6
 ** tensorflow 1.14.0
 ** keras 2.1.5
 ** GPU (GTX1070)
 
*Usage
 1. download yolo3.weights and yolov3.cfg 
 2. run "convertt.py  -w yolov3.cfg yolov3.weights model_data/yolo_weights.h5"
 3. generate your own annotation and class name file and place them into model_data folder
 
 format: path/to/img1.jpg box_left,box_top, box_right, box_bottom, class_label
 
 4. generate your anchlor box estimates on your training dataset by running: python kmeans.py
 5. model training:  python train.py
 6. modfel testing;  python image_detect.py
 
 
   
 
