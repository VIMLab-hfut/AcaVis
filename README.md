# Our model-----ClusterNet

ClusterNet provides a differentiable k-means clustering layer which is used as a building block for solving graph optimization problems. 

# Examples of running the experiments

Example running the single-graph experiment for the community detection problem on the cora dataset:

```
python ourtest.py
```

# Dependencies

The Dockerfile in the main directory builds the environment that was used to run the original experiments, with the exception of [pygcn](https://github.com/tkipf/pygcn/tree/master/pygcn), which needs to be downloaded and installed separately. For reference, the individual dependencies are:

* PyTorch (tested on version 1.2)
* networkx (tested on version 2.3)
* igraph (tested on version 0.7.1). This is optional; only used to accelerate pre-processing operations.
* [pygcn](https://github.com/tkipf/pygcn/tree/master/pygcn)
* sklearn (tested on version 0.21.3)
* numpy (tested on version 1.16.5)
