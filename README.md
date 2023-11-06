# Sign-language-detection-and-real-time-translation using YOLO v5



**Make sure to make a new branch if you want to train the model**

## How to install:
1. clone this rep ( choose the main/master branch to train the model yourselves or v1 branch to see the results )
2. create a new environment and pip install requirements.txt
3. run the commands below using full absolute paths acoording to the directory in which you cloned and make sure its enclosed by single quotes ( also use / instead of \ )<br>

### Training:
```text

python '.yolov5/train.py' --img 416 --batch 16 --epochs 300 --data './yolov5/data.yaml' --cfg '.yolov5/models/custom_yolov5s.yaml' --weights 'yolov5s.pt' --name yolov5s_results  --cache

```

### Detect:
```text

python '.yolov5/detect.py' --weights '.yolov5/runs/train/yolov5s_results/weights/best.pt' --img 416 --conf 0.5 --source '.test/images'

```

### Run:
```text

python '.yolov5/run.py'

```

## Branch v1:
- It has the 1st training results 
- You can run the model
- high overfitting

***Inference***: needs a **bigger**, **well labelled** dataset
