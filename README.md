# Graph_Anonymization

Graph anonymization algorithm is developed to protect privacy of users in social networks when the network is plotted as a dataset, by obfuscating the said network.
The obfuscation process is performed in such a way that the integrity of connections is still retained.
In obfuscating a network the cruicial points to consider are cut-vertices, bridges, degree of freeedom of each nodes.
A cut vertex is a vertex that when removed (with its boundary edges) from a graph creates more components than previously in the graph.
Cut vertices are important points to protect in a network since the number of connections are higher.
Those points are protected by adding dummy nodes and relationships inside the network.
A bridge is defined as an edge which, when removed, makes the graph disconnected (or more precisely, increases the number of connected components in the graph)
A bridge is again important since attacking a particular crucial connection will affect the entire network.
The said bridge is protected by creating adjacent nodes through which connections are still maintained.

# Running The Algorithm

The said algorithm is tested with several networks downloaded from verious sources like:

1) Karate Club Dataset-http://vlado.fmf.uni-lj.si/pub/networks/data/Ucinet/UciData.htm
2) Jazz Arenas Dataset-https://nrvis.com/download/data/misc/arenas-jazz.zip
3) Facebook Network -Attached with repository
4) Email Dataset - Attached with repository


Find notebook named algorithm20211017.ipynb and run all cells to extract network obfucated for karate.gml and email.csv. 
The obfuscated network can be downloaded to graph edge list file(.gexf) format.
The algorithm can be applied to any network to get the obfuscated network.
