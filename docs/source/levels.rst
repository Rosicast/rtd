.. _levels:

======
Levels
======

Levels

* Graph-level
    * Classification
        * Categorize different graph
        * e.g. Molecule property prediction
    * Generation
        * e.g. Drug discovery
    * Evolution
        * e.g. gPhysical simulation
    * Examples
        * Drug discovery 
            * Nodes: Atoms
            * Edges: Chemical bonds
        * `Antibiotic Discovery <https://www.sciencedirect.com/science/article/pii/S0092867420301021>`_
        * `GCPN <https://arxiv.org/pdf/1806.02473.pdf>`_
        * `Physics simulation <https://arxiv.org/pdf/2002.09405.pdf>`_
            * Nodes: Particles
            * Edges: Interaction between particles
* Subgraph-level (community)
    * Clustering
        * Detect if nodes from a community
        * e.g. social circle detection
    * Examples
        * Traffic prediction
            * Nodes: Road segments
            * Edges: Connectivity between road segments
            * Prediction: Time of arrival (ETA)
* Node-level
    * Classification
        * Predict a property of a node
        * e.g. Categorize online users / items
    * Examples
        * AlphaFold
            * Key idea: spatial graph
            * Nodes: Amino acids in a protein sequence
            * Edges: Proximity between amino acids (residues)
* Edge-level
    * Link prediction
        * Predict whether there are missing links between two nodes
        * e.g. Knowledge graph completion
    * Examples
        * `PinSage <https://arxiv.org/pdf/1806.01973.pdf>`_
            * Recommender systems
            * Nodes: users and items
            * Edges: user-item interactions
        * `De novo <https://arxiv.org/pdf/1802.00543.pdf>`_
            * Drug side effects
            * Nodes: Drugs and proteins
            * Edges: Interatctions

