# Amazon product co-purchasing network and ground-truth communities

Url: [https://snap.stanford.edu/data/com-Amazon.html](https://snap.stanford.edu/data/com-Amazon.html)

Network was collected by crawling Amazon website. It is based on Customers Who Bought This Item Also Bought feature of the Amazon website. If a product i is frequently co-purchased with product j, the graph contains an undirected edge from i to j. Each product category provided by Amazon defines each ground-truth community.

We regard each connected component in a product category as a separate ground-truth community. We remove the ground-truth communities which have less than 3 nodes. We also provide the top 5,000 communities with highest quality which are described in our paper. As for the network, we provide the largest connected component.

Dataset | statistics
--------|-----------
Nodes	| 	334863
Edges	| 	925872
Nodes in largest WCC	| 	334863 (1.000)
Edges in largest WCC	| 	925872 (1.000)
Nodes in largest SCC	| 	334863 (1.000)
Edges in largest SCC	| 	925872 (1.000)
Average clustering coefficient 	0.3967
Number of triangles 	667129
Fraction of closed triangles 	0.07925
Diameter (longest shortest path) 	44
90-percentile effective diameter 	15


## Source (citation)

J. Yang and J. Leskovec. Defining and Evaluating Network Communities based on Ground-truth. ICDM, 2012.


## Files
File | Description
-----|------------
com-amazon.ungraph.txt.gz | Undirected Amazon product co-purchasing network
com-amazon.all.dedup.cmty.txt.gz | Amazon communities
com-amazon.top5000.cmty.txt.gz | Amazon communities (Top 5,000)