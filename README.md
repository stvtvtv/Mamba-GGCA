Dataset
```bash
链接: https://pan.baidu.com/s/11PXjoCrTwjGibd9Vc1aI4g?pwd=1234 提取码: 1234
```
Run the code, and you need to select the model you want. The commented sections refer to the model's YAML file and the training file.
train
```bash
from ultralytics import YOLO

if __name__ == '__main__':

    model = YOLO(r'ltralytics\cfg\models\v8\yolov8.yaml')    # 	Original
    # yolov8mbgcsa2.yaml   	Mamba GCSA
    # yolov8gcsamb.yaml    	Mamba GGCA
    # yolov8ggca.yaml    	  GGCA
    # yolov8gcsa.yaml   	  GCSA


    model.train(data=r"data.yaml",  
                epochs=3, imgsz=640, batch=1, workers=2)
```

But you need to modify the dataset location manually.

The role of txt.py is to test various model parameters

display dataset categories.

```bash
  0: Spotted chela
  1: Wax cicada
  2: greenhopper
  3: stinkbug
  4: melon fly
  5: mole cricket
  6: red spider mite
  7: ladybird
  8: vine hawk moth
  9: grub
  10: dichocrocis punctiferalis
  11: longicorn
  12: snout beetle
  13: aphid
  14: leafhopper
  15: leaf beetle
  16: Odontoides leucoides
  17: larva
  18: Mildew
  19: Bacterialblight
  20: Blast
  21: Brownspot
```

