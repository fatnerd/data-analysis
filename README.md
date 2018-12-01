# data-analysis
這是我學習python data analysis的筆記
有想補充的東西都可以開issue 
歡迎補充~
# numpy
是python list的函數庫
安裝:terminal->pip3 install numpy
只能存同一種型態(True->1,False->0),eg:[1,2,4]

## 用np取代函數庫numpy 
import numpy as np

## Create np_height from np_baseball 
#只擷取第一列 
np_height = np.array(np_baseball[:,0])

## Print out the mean of np_height
print(np.mean(np_height))

## Print out the median of np_height
print(np.median(np_height))

## Print out correlation between first and second column. 
corr = np.corrcoef(np_baseball[:,0], np_baseball[:,1])
print("Correlation: " + str(corr))

## 計算standard_deviation
np.std()

## Print out the 50th row of np_baseball
print(np_baseball[49,:])

## Select the entire second column of np_baseball: np_weight
np_weight = np_baseball[:,1]

## Print out the shape of np_baseball
print(np_baseball.shape)

# matplotlib
視覺化資料
## import函數庫
import matplotlib.pyplot as plt
## 畫折線圖
plt.plot(x,y)
## 加入x,y軸定義
plt.xlabel('')
plt.ylabel('')
## 加入圖的標題
plt.title('')
## yticks y軸組距
plt.yticks([舊的][新的])

## 加入幾筆資料
例如:
year = [2010,2013,2016,2019]
year = [2021,2024] + year
## 顯示圖
plt.show()
## scatter散點圖
plt.scatter(x,y)
# histogram 直方圖
## import函數庫
import matplotlib.pyplot as plt

## bins是直方圖條的個數
plt.hist(nameoflist,bins="")
