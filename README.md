# data-analysis
# numpy
是python list的函數庫
安裝:terminal->pip3 install numpy
只能存同一種型態(True->1,False->0),eg:[1,2,4]

# 用np取代函數庫numpy 
import numpy as np

# Create np_height from np_baseball 
#只擷取第一列 
np_height = np.array(np_baseball[:,0])

# Print out the mean of np_height
print(np.mean(np_height))

# Print out the median of np_height
print(np.median(np_height))

# Print out correlation between first and second column. 
corr = np.corrcoef(np_baseball[:,0], np_baseball[:,1])
print("Correlation: " + str(corr))

# 計算standard_deviation
np.std()

# Print out the 50th row of np_baseball
print(np_baseball[49,:])

# Select the entire second column of np_baseball: np_weight
np_weight = np_baseball[:,1]

# Print out the shape of np_baseball
print(np_baseball.shape)
