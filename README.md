# Keras_MNIST 手寫影像辨識,可辨識 0~9的手寫數字
![image](https://user-images.githubusercontent.com/78743080/151687335-58ebda06-565c-4bd5-b27d-e1c6131689a1.png)


## Model
- MLP
- CNN

MLP VS CNN
||reshape|說明|
|---|---|---|
|MLP|image.reshape(60000,784)|多元感知器因直接送進神經元處理，所以reshape轉換為60000筆，每一筆有784個數字，作為784個神經元的輸入
|CNN|image.reshape(60000,28,28,1)|CNN因為必須先進行卷積與池化運算，所以必須保持影像的維度，所以reshape轉換為60000筆，每一筆有28X28X1的影像

## Results
|Measures |MLP|CNN|
 |---|---|---|
|Accurracy| 0.98|0.99|

## Value
1. 資料觀察: 觀察影像資料
![image](https://user-images.githubusercontent.com/78743080/151687409-af92d8ec-308a-47c3-8c70-7c44ed44aa93.png)
2. 資料前處理: 影像資料正規化
3. 混淆矩陣: 全面性觀察
![image](https://user-images.githubusercontent.com/78743080/151687420-e88aea2f-023f-4ea5-8189-4639a98fb977.png)
4. 參數計算： 包含CNN模型參數的計算，了解model建立過程


