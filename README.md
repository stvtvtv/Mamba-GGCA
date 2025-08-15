数据集
```bash
链接: https://pan.baidu.com/s/11PXjoCrTwjGibd9Vc1aI4g?pwd=1234 提取码: 1234
```
运行代码， 需要你选择想要的模型  下面注释的就模型yaml文件
train文件
```bash
from ultralytics import YOLO

if __name__ == '__main__':

    model = YOLO(r'ltralytics\cfg\models\v8\yolov8.yaml')    # 1	Original
    # yolov8mbgcsa2.yaml   5	Mamba GCSA
    # yolov8gcsamb.yaml    6	Mamba GGCA1
    # yolov8ggca.yaml    2	  GGCA
    # yolov8gcsa.yaml    4	  GCSA

    # 模型训练
    model.train(data=r"data.yaml",  # 训练数据配置文件
                epochs=3, imgsz=640, batch=1, workers=2)
```

但是数据集位置还要自己修改

txt.py 作用
可以测试模型各个参数

数据集展示类别
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

