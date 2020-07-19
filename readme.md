# weapon detector

**Install**
1. Download and place in the weapons folder and unzip. http://pyimg.co/gdxyi
2. Download the pre-trained network and place it in the main directory. https://github.com/fizyr/keras-retinanet/releases/download/0.5.1/resnet50_coco_best_v2.1.0.h5
3. Download the output file and place it in the main directory. https://drive.google.com/file/d/1fNtDoOFO4ViPjEi9cFyr_HTjeCiYJwgH/view?usp=sharing
4. If you have not yet installed the retinanet, [click here](Installing Keras RetinaNet.pdf).

## Predict just an image
run:\
```python predict.py --model output.h5 --labels weapons/retinanet_classes.csv --image weapons/images/armas_1.jpg --confidence 0.5```

## Predicting batch images
run:\
```python predict_batch.py --model output.h5 --labels weapons/retinanet_classes.csv --input weapons/images/ --output output```

OUTPUT:\
![Alt text](output/armas_1.jpg?raw=true "Title")
![Alt text](output/armas_2.jpg?raw=true "Title")
![Alt text](output/armas_3.jpg?raw=true "Title")
