# Neural-Network-Pruning
Here two different methods for pruning a fully connected neural network on Fashion MNIST dataset are presented.

Please open for_ai_final.ipynb file in this repository on Google Colab and run all the cells sequentially.

An introduction on the implemented pruning methods (source: for.ai)

Given a layer of a neural network there are two well-known ways to prune it:
  - Weight pruning: set individual weights in the weight matrix to zero. This corresponds to deleting connections as in the figure above.
    Here, to achieve sparsity of k% we rank the individual weights in weight matrix W according to their magnitude (absolute value) |wi,j|, and then set to zero the smallest k%.
  - Unit/Neuron pruning: set entire columns to zero in the weight matrix to zero, in effect deleting the corresponding output neuron.
    Here to achieve sparsity of k% we rank the columns of a weight matrix according to their L2-norm and delete the smallest k%.