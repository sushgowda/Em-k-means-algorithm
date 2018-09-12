# Em-k-means-algorithm
import matplotlib.pyplot as plt
from sklearn import datasets
from sklearn.cluster import KMeans
import sklearn.metrics as sm
import pandas as pd
import numpy as np
%matplotlib inline

iris=datasets.load_iris()

X=pd.DataFrame(iris.data)
X.columns=['Sepal_length','Sepal_Width','Petal_Length','Petal_width]
y=pd.DataFrame(iris.target)
y.columns=['Targets']
plt.figure(gifsize=(14,7))
colormap=np.array(['red','lime','black'])
plt.subplot(1,2,1)
plt.scatter(Z.Petal_Length,X.PEtal_Width,c=colormap[y.Targets],s=40)
plt.title('Sepal')

plt.subplot(1,2,2)
plt.scatter(X.Petal_Length,X.Petal_Width,c=colormap[y.Targets],s=40)
plt.title('Petal')
