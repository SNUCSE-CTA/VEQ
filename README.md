# VEQ
Versatile Equivalences: Speeding up Subgraph Query Processing and Subgraph Matching  
VEQ_S: VEQ for subgraph search  
VEQ_M_100k: VEQ for subgraph matching, which finds up to 100,000 embeddings  
  
Usages:  
./VEQ_S -dg [data graph file] -qg [query graph file] -o [output file]  
./VEQ_M_100k -dg [data graph file] -qg [query graph file]  

Example Usages:  
./VEQ_S -dg subgraphSearchData/COLLAB.gfu -qg subgraphSearchQuery/COLLAB/randomwalk/8/q0.gfu -o output.txt  
./VEQ_M_100k -dg subgraphMatchingData/human.gfu -qg subgraphMatchingQueryRevision/human/sparse/10/q0.gfu  

Input File Format:  
[graph ID]  
[the number of vertices (n)]  
[the label of v_1]  
...  
[the label of v_n]  
[the number of edges (m)]  
[vertex ID of e_1] [vertex ID of e_1]  
...  
[vertex ID of e_m] [vertex ID of e_m]  
  
Example Input:  
#0  
3  
1  
0  
0  
2  
0 1  
1 2  
