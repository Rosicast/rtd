.. _representation:

====================
Graph representation
====================

Choice of the proper network representation of a given domain/problem determines our ability to use networks successfully: In some cases, there is a unique, unambiguous representation. In other cases, the representation is by no means unique. The way you assign links will determine the nature of the question you can study

* Components
    * Objects: Nodes :math:`N`
    * Interactions: links and edges :math:`E`
    * System: network, graph  :math:`G(N,E)`
* Direction
    * Undirected
        * Links: undirected, symmetrical, reciprocal
    * Directed
        * Links: directed, arcs
* Heterogeneous Graphs
    * Defined:              :math:`G=(V,E,R,T)`
    * Nodes with node types :math:`v_i \in V`
    * Edges with relation types :math:`(v_i, r, v_j) \in E`
    * Node type :math:`T(v_i)`
    * Relation type :math:`r \in R`
    * Examples
        * Biomedical knowledge graph
            * Example node: Migraine 
            * Example edge: (fulvestrant, Treats, Breast Neoplasms)
            * Example node type: Protein
            * Example edge type (relation): Causes
        * Academic Graphs
            * Example node: ICML 
            * Example edge: (GraphSAGE, NeurIPS) 
            * Example node type: Author 
            * Example edge type (relation): pubYear
* Node degree, :math:`k_i`
    * Undirected
        * The number of edges adjacent to node i
        * Avg. degree: :math:`\bar{k} = <k> = \frac{2E}{N}`
    * Directed
        * In-degree: :math:`k_C^{in} = 2`
        * Out-degree :math:`k_C^{out} = 1`
        * :math:`k_C = 3`
        * :math:`\bar{k} = \frac{E}{N}`
        * :math:`\bar{k}^{in} = \bar{k}^{out}`
* Bipartite graph
    * A graph whose nodes can be divided into two disjoint sets U and V such that every link connects a node in U to one in V; that is, U and V are independent sets
    * Examples
        * Authors-to-Papers
        * Actors-to-Movies
        * Users-to-Movies
        * Recipes-to-Ingredients
    * Folded networks
        * Author collaboration networks
        * Movie co-rating networks
* Adjacency Matrix
    * :math:`A_{ij} = 1` if there is a link from node :math:`i`  to node :math:`j`
    * :math:`A_{ij} = 0` otherwise
    * Most real-world networks are sparse, therefore, an adjacency matrix is filled with zeros!
* Edge list
    * Represent graph as a list of edges
    * Example
        * (2, 3)
* Adjacency list
    * Easier to work with if a network is large and sparse
    * Allows us to retrieve all neighbors of a given node quickly
    * Example:
        * 1:
        * 2: 3, 4
        * 3: 2, 4
* Node and edge Attributes
    * Weight
    * Ranking
    * Type
    * Sign
    * Others
* Types of Graphs
    * Weighted 
        * Collaboration
        * Internet
        * Roads
    * Unweighted
        * Friendship
        * Hyperlink
    * Self-edges (self-loops)
        * Proteins
        * Hyperlink
    * Multigraph
        * Communication
        * Collaboration
