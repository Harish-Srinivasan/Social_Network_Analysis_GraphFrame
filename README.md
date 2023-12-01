# Social_Network_Analysis_GraphFrame

Reddit dataset is analysed using PySpark GraphFrame using queries and algorithms. The following queries are answered:

1. Top 5 nodes with highest outdegree and count of outgoing edges: 

+---------------+---------+
|id             |outDegree|
+---------------+---------+
|subredditdrama |4665     |
|circlebroke    |2358     |
|shitliberalssay|1968     |
|outoftheloop   |1958     |
|copypasta      |1824     |
+---------------+---------+

2. Top 5 nodes with the highest indegree and count of incoming edges:

+--------------+--------+
|id            |inDegree|
+--------------+--------+
|askreddit     |7329    |
|iama          |3694    |
|pics          |2779    |
|writingprompts|2490    |
|videos        |2446    |
+--------------+--------+

3. PageRank for each of the nodes and output the top 5 nodes with the highest PageRank values:

+-----------------+------------------+
|               id|          pagerank|
+-----------------+------------------+
|        askreddit| 579.1150697170434|
|             iama| 474.7547863573387|
|           videos| 425.0334335188542|
|videos_discussion|329.51376047756264|
|             pics|249.84530454363428|
+-----------------+------------------+

4. Run the connected components algorithm on it and find the top 5 components with the largest number of nodes.

+------------+-----+
|   component|count|
+------------+-----+
|           0|26492|
| 77309411334|    5|
|240518168606|    5|
|171798691843|    5|
|695784702079|    4|
+------------+-----+

5. Run the triangle counts algorithm on each of the vertices and output the top 5 vertices with the largest triangle count: 

+-----+--------------+
|count|            id|
+-----+--------------+
|30139|     askreddit|
|24162|subredditdrama|
|23370|          iama|
|14624|  outoftheloop|
|11924|        videos|
+-----+--------------+

