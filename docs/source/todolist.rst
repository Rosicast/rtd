.. _todolist:

========
Todolist
========

Definitions

* NP-hard
* i.i.d 
* BFS (breadth-first search)
Outline

* Traditional methods
   * Graoglets
   * Graph Kernels
* Methods for node embeddings
   * GCN
   * GraphSAGE
   * GAT
   * Theory of GNNs
* Knowledge graphs and reasoning
   * TransE
   * BetaE
* Deep generative models for graphs
   * GraphRNN
   
Classic Graph ML Tasks

* Node classification: Predict a property of a node
    * Example: Categorize online users / items
* Link prediction: Predict whether there are missing links between two nodes
    * Example: Knowledge graph completion
* Graph classification: Categorize different graphs
    * Example: Molecule property prediction
* Clustering: Detect if nodes form a community
    * Example: Social circle detection
* Other tasks:
    * Graph generation: Drug discovery
    * Graph evolution: Physical simulation

* adjacency list

Tasks

* Node-level
* Link-level
* Graph-level

graphs

* Directed graph
* Undirected graph

Node-level

* Importance-based features
    * Node degree
    * Node centrality
        * Eigenvector centrality
        * Closeness centrality
        * Betweenness centrality
* Structure-based features
    * Node degree
    * Clustering coefficient
    * Graphlets
        * Induced subgraph
        * Graph Isomorphism
        * Graphlet Degree Vector

Link-level features

* Distance-based features
    * Shortest path length
* Local neighborhood overlap
    * Common neighbors
    * Jaccard's coefficient
    * Adamic-Adar index
* Global neighborhood overlap
    * Katz index

Graph-level features

* Kernel methods
    * Graph Kernels
        * Graphlet Kernel
        * Weisfeiler-Lehman Kernel
            * Color Refinement
            * Bag-of-colors
        * Random-walk Kernel
        * Shortest-path graph Kernel

Node embeddings

Why?
    Efficient task-independent feature learning for machine learning with graphs

Different notation of Node similarity

* Naive: similar if two nodes are connected
* Neighborhood overlap
* Random walk approaches

* Encoder and Decoder
    * Shallow encoding
        * DeepWalk
        * Node2vec
            * BFS: Micro-view of neighborhood
            * DFS: Macro-view of neighborhood
* Random DeepWalk
* Unsuoervised feature learning
    * Negative sampling

Embedding Entire Graph

Goal
    .. math:: \text{Want to embed a subgraph or an entire graph G. Graph embedding:} Z_G
Tasks
    * Classifying toxic vs non-toxic molecules
    * Identifying anomalous graphs

Approaches

* Simple approache: Sum the node embeddings
* Virtual node
* Anonymous Walk embeddings
    * Represent the graph as a probability distribution over these walks.
    * Sampling Anonymous Walks
    * Learn Walk embeddings

.. math:: \text{How to use embeddings } Z_i \text{ of nodes}

* Clustering or community detection
* Node classification
* Link prediction
    * Concatenate
    * Hadamard
    * Sum/Avg
    * Distance
* Graph classification

PageRank

Web as a (directed) graph:
* Nodes = web pages
* Edges = hyperlinks

Link analysis approaches

* PageRank
* Personalized PageRank (PPR)
* Random Walk with Restarts

Matrix Factorization and Node embeddings

Message passing and Node classification

Correlations exist in networks

* Homophily
* Influence

Classification with network data

Motivation

* Similar nodes are typically close together or directly connected in the network
    * Guilt-by-association: If I am connected to a node with label X, then I am likely to have label X as well.
* Classification label of a node v in network may depend on: Feature of v, labels of the nodes in v's neighborhood, and features of the nodes in v's neighborhood


