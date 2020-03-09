# self_organising_maps

In this repository the Self-Organising Map (SOM) is implemented from scratch. In this algorithm instead of having layers of neurons, we have a grid with all the neurons (feature mapping). The input space is high dimensional and the output space is low dimensional.


<img src="https://miro.medium.com/max/1310/1*QG7afWQKjY3IpezhNQMzBg.png"/>


The SOM algorithm is a CL algorithm (unsupervised), so that one neuron is chosen as the winner, but when its weights are updated, so are those of its neighbours, although to a lesser extent. Neurons that are not within the neighbourhood are ignored. The steps of the algorithm for each training sample are the following:
1. Calculate the similarity (euclidean distance) between the input pattern and the weights arriving at each output node.
2. Find the most similar node; often referred to as the *winner*.
3. Select a set of output nodes which are located close to the winner in the *output grid*. This is called *neightbourhood*.
4.  Update the weights of all nodes in the neighbourhood such that their weights are moved closer to the input pattern. 
