# HetGDCN
An implement of our paper "Diffusion-based Graph Convolution Networks for Heterogeneous Graphs using Type-Adaptive Normalization" (Submission for TheWebConf 2023).

Thank you for your interest in our works!  

# Motivation
(1) Diffusion-based GCNs have made success on analyzing graph data thanks to their robustness of structural noise.
    However, these diffusion-based GCNs assume that graphs are either homophilic or heterophilic.
(2) We find out that heterogeneous graphs are neither homophilic nor heterophilic.  

Our paper present a novel type-adaptive (de)normalization to analyze heterogeneous graphs by decoupling type- and content- information of nodes.
![type_adaptive](https://user-images.githubusercontent.com/37531907/197387808-7bc26a92-6379-4450-8a7b-a39a0cdea4de.PNG)

In this paper, we assume that connected nodes have similar content information.
With the assumption, our HetGDCN diffuses content information with graph diffusions.
Then, we recombine type- and content- information.
![overview](https://user-images.githubusercontent.com/37531907/197387805-0bb48489-284c-4fc8-af92-c014dc6f62c0.PNG)

# Dependencies
Recent versions of the following packages for Python 3 are required:

* Anaconda3
* Python 3.7.11  
* Pytorch 1.10.2  
* torch_geometric 2.0.4  
* torch_scatter 2.0.9  

# Easy Run
> python main.py --dataset=DBLP --mode=appnp
