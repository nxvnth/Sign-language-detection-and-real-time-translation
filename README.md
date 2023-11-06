# Sign-language-detection-and-real-time-translation
using YOLO v5

ignore the first 74 commits 
if any file is missing, inform

1. clone this rep 
2. create a new environment and pip install requirements.txt
3. run the command below using full absolute paths acoording to the directory in which you cloned and make sure its enclosed by single quotes

python 'E:\signnew\Sign-Language-Detection-and-Translation-using-YOLOV5\yolov5\train.py' --img 416 --batch 16 --epochs 300 --data 'E:\signnew\Sign-Language-Detection-and-Translation-using-YOLOV5\data.yaml' --cfg 'E:\signnew\Sign-Language-Detection-and-Translation-using-YOLOV5\yolov5\models\custom_yolov5s.yaml' --weights 'yolov5s.pt' --name yolov5s_results  --cache
