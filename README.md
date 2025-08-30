# CNN-Semi-Supervised-Learning
李宏毅 ML 作業筆記 3: 食物分類，這裡使用的資料集是 food-11，建立一個用於影像分類的捲積神經網絡，利用提供的未標記資料來獲得更好的結果。 

## 模型性能
- Model1驗證集準確率：82%
- Model4驗證集準確率：82%
- 在Kaggle上Model1測試集準確率：80%
- 在Kaggle上Model4測試集準確率：82.5%
- 在Kaggle上Model5測試集準確率：83%

* Run `Model1.ipynb`, `Model4.ipynb`, respectively.

This will generate `model1.ckpt`, `model4.ckpt` . Note that you must execute these models orderly, since some model is retrained from previous models using unlabeled data (semi-supervised). 

* Run `Ensemble.ipynb`.

This will ensemble model1, model4 by voting. The resulting are saved in `model5.ckpt`.
