# single-object-detection-yolov3-keras

*Environments

 * python 3.6
 * tensorflow 1.14.0
 * keras 2.1.5
 * GPU (GTX1070)
 * OpenCV 4.1.1
 
*Usage
 1. download yolo3.weights and yolov3.cfg 
 2. run "convert.py  -w yolov3.cfg yolov3.weights model_data/yolo_weights.h5"
 3. generate your own annotation (e.g., train.txt) in the current project folder
   * for example:
    format: path/to/img1.jpg box_left,box_top,box_right,box_bottom,class_label (Note a space between .jpg file and box_left and no space betwen ",")
 4. generate a class name file and place it into model_data folder
    * For single object, class-label set as 0, class_name.txt containing the single object name
 5. generate your anchlor box estimates on your training dataset by running: python kmeans.py
 6. model training:  python train.py
 7. modfel testing:  python image_detect.py
 
 
   
 
