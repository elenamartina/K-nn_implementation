# k-Nearest Neighbours Algorithm

My implementation of the k-Nearest Neighbours algorithm.


## Parameters
   * `X` :  the training data *(required)*
   * `y` :  the training labels *(required)*
   * `X_` :  the testing data *(required)*
   * `n_neighbours` :  the number of neighbours *(default = 5)*
   * `distance metric` :  the distance function to be used *(default = “minkowski′′)*
   * `p` :  power parameter of the Minkowski distance. *(default = 2)*
   * `breaktie metric` :  the metric to use when a tie occurs *(default = “smallest′′)*
   * `weights method` :  the method to use to weight the neighbours *(default = “uniform′′)*
   
## Distance Metrics implemented

* Minkowski 
* Euclidean
* Manhattan
* Chebyshev
* Hassanat
   
## Tie Breaking
If two or more different classes appear to be the most frequent, the algorithm calls the `break tie()` function, which will deal with the tie in the method defined in the parameter `breaktie_metric`, and return the predicted label.

#### Metrics implemented:
* `smallest` *(default)*: picks the first class it finds (the smallest index) among tied groups;
* `nearest`: picks the class with the nearest neighbour among tied groups;
* `random`: randomly picks a class among tied group.
