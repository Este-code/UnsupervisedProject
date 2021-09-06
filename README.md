# UnsupervisedProject

This dataset contains socio-economic and health factors that determine the overall development of countries. The purpose of the dataset is to help a charity fighting poverty to identify groups of countries where it is needed most.

**Task**: Which countries can be grouped together and have the highest need of help from the charity?

**Heatmap**

![alt text](https://github.com/Este-code/UnsupervisedProject/blob/main/image/heatmap.png)

k means clustering based on the correlation between child moratility and total fertility
I checked which features have the highest correlation based on the heatmap.
The highest one was the correlation between income and gdpp; but when I plotted them, the clustering was not so clear.
Therefore I tried the second highest correlation, which is the one between child moratlity and total fertility, and the result was very clear.

![alt text](https://github.com/Este-code/UnsupervisedProject/blob/main/image/graph.png)

**Model**

I decided to set 3 as number of cluster, to underline the countries who need help from the ones that partially need help, and the ones that do not need help.

![alt text](https://github.com/Este-code/UnsupervisedProject/blob/main/image/graph1.png)

**Result**

This is the result of the clustering.

![alt text](https://github.com/Este-code/UnsupervisedProject/blob/main/image/country.png)

**Recommendations**

Clustering based on 2 features which highly correlate isn't necessarily the best way to go, as there will be very little difference between the columns if they correlate highly. If anything, you want to exclude features which highly correlate with other features. You could instead include all the features in your data into the clustering.
Scaling the data to perhaps could improve the model performance.
