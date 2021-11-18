# GNN for Position Reconstruction of the XENON Events

The XENON Experiment was established to study potential dark matter candidates. It is a cylinder full of liquid Xenon with vacuum tubes (to detect photons) aligned in a hexagonal arrangement at the top and the bottom faces.

This hexagonal arrangement piqued the community’s interest to experiment with graph neural networks. I experimented with different graph neural network layers to come up with a GNN design that can successfully reconstruct the position of the collision happening in the detector.

This basically can be modeled as a graph regression problem.

 ## Requirements
 1. ```tensorflow```
 2. ```spektral```
 3. ```numpy```


 ## Usage
Each interactive python file consisits of an implementation fo a iddferent kind of GNN on the XENON dataset. Due to copyright reasons, the network could not be made public. A sample notebook displays the usage on the QM9 dataset (a graph regression problem).

## GNN Layers Experimented With

#### 1. ECCConv
#### 2. Graph Attention Layers
#### 3. MinCutPool
#### 3. Graph Convolutional Layers

## Results
The Graph Neural Network (with 200k trainable parameters) obtained an RMSE of 1.936 cm. It outperformed a Convolutional Neural Network (with 5 million trainable parameters) by 12%, and the original software used for positon reconstruction by XENON (straxen) by 67%.
