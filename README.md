# Sign-language-detection-and-real-time-translation
using YOLO v5

ignore the first 77 commits 
if any file is missing, inform
Make sure to make a new branch if you want to train the model 

1. clone this rep ( choose the main/master branch to train the model yourselves or v1 branch to see the results )
2. create a new environment and pip install requirements.txt
3. run the command below using full absolute paths acoording to the directory in which you cloned and make sure its enclosed by single quotes (also use / instead of \)

   For eg:

training
python 'E:/signnew/Sign-Language-Detection-and-Translation-using-YOLOV5/yolov5/train.py' --img 416 --batch 16 --epochs 300 --data 'E:/signnew/Sign-Language-Detection-and-Translation-using-YOLOV5/data.yaml' --cfg 'E:/signnew/Sign-Language-Detection-and-Translation-using-YOLOV5/yolov5/models/custom_yolov5s.yaml' --weights 'yolov5s.pt' --name yolov5s_results  --cache

detect
python 'E:/signnew/Sign-Language-Detection-and-Translation-using-YOLOV5/yolov5/detect.py' --weights 'E:/signnew/Sign-Language-Detection-and-Translation-using-YOLOV5/yolov5/runs/train/yolov5s_results10/weights/best.pt' --img 416 --conf 0.5 --source 'E:/signnew/Sign-Language-Detection-and-Translation-using-YOLOV5/test/images'

run
python 'E:/signnew/Sign-Language-Detection-and-Translation-using-YOLOV5/yolov5/run.py'

Branch v1:
It has the 1st training results 
You can run the model
high overfitting
Inference: need better, bigger, well labelled dataset
