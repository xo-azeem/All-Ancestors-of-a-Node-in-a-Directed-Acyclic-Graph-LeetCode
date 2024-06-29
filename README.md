# All Ancestors of a Node in a Directed Acyclic Graph

LeetCode Q # 2192.

You are given a positive integer n representing the number of nodes of a Directed Acyclic Graph (DAG). The nodes are numbered from 0 to n - 1 (inclusive).

You are also given a 2D integer array edges, where edges[i] = [fromi, toi] denotes that there is a unidirectional edge from fromi to toi in the graph.

Return a list answer, where answer[i] is the list of ancestors of the ith node, sorted in ascending order.

A node u is an ancestor of another node v if u can reach v via a set of edges.

Example 1:

<div align = "center">

![image](https://github.com/xo-azeem/All-Ancestors-of-a-Node-in-a-Directed-Acyclic-Graph-LeetCode/assets/171427226/bdabfa88-c657-4af7-88c5-de177abc2057)
  
</div>

> Input: n = 8, edgeList = [[0,3],[0,4],[1,3],[2,4],[2,7],[3,5],[3,6],[3,7],[4,6]]</br>
> Output: [[],[],[],[0,1],[0,2],[0,1,3],[0,1,2,3,4],[0,1,2,3]]</br>
> Explanation:</br>
> The above diagram represents the input graph.</br>
> - Nodes 0, 1, and 2 do not have any ancestors.</br>
> - Node 3 has two ancestors 0 and 1.</br>
> - Node 4 has two ancestors 0 and 2.</br>
> - Node 5 has three ancestors 0, 1, and 3.</br>
> - Node 6 has five ancestors 0, 1, 2, 3, and 4.</br>
> - Node 7 has four ancestors 0, 1, 2, and 3.</br>

Example 2:

<div align = "center">

![image](https://github.com/xo-azeem/All-Ancestors-of-a-Node-in-a-Directed-Acyclic-Graph-LeetCode/assets/171427226/bfd5c4d9-3501-462f-931a-7fe8519e1ccf)
  
</div>

> Input: n = 5, edgeList = [[0,1],[0,2],[0,3],[0,4],[1,2],[1,3],[1,4],[2,3],[2,4],[3,4]]</br>
> Output: [[],[0],[0,1],[0,1,2],[0,1,2,3]]</br>
> Explanation:</br>
> The above diagram represents the input graph.</br>
> - Node 0 does not have any ancestor.</br>
> - Node 1 has one ancestor 0.</br>
> - Node 2 has two ancestors 0 and 1.</br>
> - Node 3 has three ancestors 0, 1, and 2.</br>
> - Node 4 has four ancestors 0, 1, 2, and 3.</br>

My Solution Analysis:

<div align = "center">

  ![image](https://github.com/xo-azeem/All-Ancestors-of-a-Node-in-a-Directed-Acyclic-Graph-LeetCode/assets/171427226/fa38ce1a-95df-4399-b1af-9ec1d4501be3)

  Time complexity: O(n^2).</br>Space complexity: O(n^2).
</div>
