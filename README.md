# SNS_features_dataset

Datasets of software network structure  for defect prediction.
* Came(1.0/1.4/1.6)
* Jedit(3.2/4.1/4.2/4.3)
* Lucene(2.0/2.2/2.4)
* Synapse(1.0/1.1/1.2)
* Xerces(1.2/1.3/1.4)

## defect information
defect information is obtained from tera-PROMISE repository (http://openscience.us/repo/defect/)

## metrics
32 software network structure features include 18 global network structure features and 14 ego network structure features. The 34 different software structure features were calculated by software source code.

1.Global network measures
* Degree		Nodes adjacent to a given node
* Out degree	Number of edges incoming to that node
* In degree		Number of edges outgoing from that node
* Ripple degree	Number of nodes that that node can reach along directed paths
* Average neighbor degree	Average degree of the neighborhood of that node
* Betweenness	Sum of shortest paths that pass through that node
* Pagerank		Ranking of that nodes based on the structure of the incoming links
* Clustering		Fraction of possible triangles through that node that exist
* Square clustering	Fraction of possible squares that exist at the node
* Closeness centrality	Reciprocal of the sum of the shortest path distances from that node to all other nodes
* Degree_centrality	Fraction of nodes it is connected to that node
* Out degree centrality	Fraction of nodes its outgoing edges are connected to that node
* In degree centrality	Fraction of nodes its incoming edges are connected to that node
* Betweenness centrality	Sum of the fraction of all-pairs shortest paths that pass through that node
* Load centrality	Fraction of all shortest paths that pass through that node
* Number of cliques	Number of maximal cliques for each node
* Core number	Largest value k of a k-core containing that node
* Eccentricity	Maximum distance from that node to all other nodes

2.Ego network measures
* Size	Nodes that ego is directly connected to
* Ties 	Directed ties corresponds to the number of edges
* Pairs	Unique pairs of nodes, i.e., Size×(Size−1)
* Density	Ties/Pairs
* nWeakComponents	Weak components in the ego network
* pWeakComponents	Weak components normalized by size
* 2StepReach		Nodes ego can reach within two steps normalized by Size
* 2StepPreach	2StepReach/(N-1)
* Reach_efficiency	2StepReach normalized by the sum of the size of the ego’s * * every Neighbor’s ego network
* Broker	Pairs not directly connected to each other
* nBroker	Broker normalized by the number of pairs
* nClose	Number of closed triads ego is involved in
* EgoBetweenness	Shortest paths between neighbors that pass-through ego
* nEgoBetweenness	EgoBetweenness normalized by the size of the ego network
