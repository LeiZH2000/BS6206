I do the clustering based on the trading frquency, which is in the file "clustering_based_on_frequency.ipynb". 
The features for the clustering and the result of the clustering is store in the folder "clustering_based_on_frequency"

This part we mainly focus on the trading frequency, which first calculated the time distance between the latest date and earliest day of the symbol, and then divided by the number of trading times of each symbol. Next we sum up all this values and divide them by the number of symbols.

We mainly generated 6 cluster, 2 of them are generated by ourselives and 4 genrated by the Kmeans model.

We the did some exploration towards the clustering result.
