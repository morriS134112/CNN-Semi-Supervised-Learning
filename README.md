# CNN-Semi-Supervised-Learning
李宏毅 ML 作業筆記 3: 食物分類，這裡使用的資料集是 food-11，建立一個用於影像分類的捲積神經網絡，利用提供的未標記資料來獲得更好的結果。 

## 模型性能
- 模型1驗證集準確率：82%
- 模型4驗證集準確率：82%

* Run `Model1.ipynb`, `Model4.ipynb`, respectively.

This will generate `model1.ckpt`, `model4.ckpt` and the corresponding predictions `model1.csv`,  `model4.csv`. Note that you must execute these models orderly, since some model is retrained from previous models using unlabeled data (semi-supervised). 

* Run `Ensemble1.ipynb`.

This will ensemble model1, model4 by voting. The resulting predictions are saved in `Ensemble1.csv`.

* Run `Ensemble2.ipynb`.

This will ensemble model1, model4 by fusion (averaged output from all models). The resulting predictions are saved in `Ensemble2.csv`.

* Run `Ensemble3.ipynb`.

This will ensemble Ensemble1,Ensemble2 by voting. The resulting predictions are saved in `Ensemble3.csv`.
