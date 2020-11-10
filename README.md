# DataScience
NTUST Data science 

## HW1
目標：利用每日天氣觀測樣本做訓練，給入當天的觀測數據，希望能預測隔天會不會降雨。

### 演算法
MLP 為一種監督式學習的演算法，藉由輸入特徵 X=x1,x2,.....,xm 和目標值Y，此算法將可以使用非線性近似將資料分類或進行迴歸運算。MLP 可以在輸 入層與輸出層中間插入許多非線性層。

<img src="https://github.com/shungfu/DataScience/raw/master/resources/MLP.png">

最左邊那層稱作輸入層，為一個神經元集合代表輸入的特徵。每個神經元在隱 藏層會根據前一層的輸出的結果再乘上權重，做為此層的輸入 w1x1 + w2x2 +...+ wmxm 。再使用非線性的 activation function 做轉換(例如:tanh, sigmoid, logistic... )。最終獲得輸出層的 output。

## HW2
目標：透過 19 個 attributes 去分析各個 data 是否為同一群。

### 演算法
k-means 是一種非監督式學習，且是一種 clustering 常用的方法。簡單形容 k-means 的話，就是物以類聚。 K-means 的主要算法:
1. 要先決定要分 k 群，接著隨機選 k 個點作為初始群心。
2. 將資料集中的資料，分群到最靠近自己的群心內。
3. 重新計算該群的群心。
重複 2.和 3.，直到群心不在移動時，k-means 結束。

<img src="https://github.com/shungfu/DataScience/raw/master/resources/kmeans.png">