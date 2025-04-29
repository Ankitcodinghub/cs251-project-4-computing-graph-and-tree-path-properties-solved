# cs251-project-4-computing-graph-and-tree-path-properties-solved
**TO GET THIS SOLUTION VISIT:** [CS251 Project 4 Computing Graph and Tree-path Properties Solved](https://www.ankitcodinghub.com/product/cs251-project-4-computing-graph-and-tree-path-properties-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;103243&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS251 Project 4  Computing Graph and Tree-path Properties Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<h1>Introduction</h1>
In this project you will write functions to determine various graph properties and perform explorations on trees. Graphs and trees will be represented by either adjacency lists or adjacency matrices, they will be undirected or directed, and the properties will range from simple checks to recursive traversals. The techniques you will use are common in graph problems you will encounter in later courses.

<h1>Learning Objectives</h1>
<ul>
<li>Explain the advantages and disadvantages of the different graph representations using concrete examples.</li>
<li>Demonstrate effective use of graph and tree traversal strategies. ● Perform basic linear-time operations on a directed acyclic graph.</li>
<li>Apply recursion to tree computations. In particular, to a tree problem in which an objective function is maximized.</li>
</ul>
<h1>Definitions and Notations</h1>
Assume graph G = (V, E) has n vertices and m edges with V = {0,1,2, … , n-1}. All graphs are simple graphs. Note that (u,v) represents an undirected edge or the edge from u to v in a directed graph. Do not make any assumption about the connectivity of a given graph.

Problems will specify which graph representation to use:

<strong>Adjacency Matrix M</strong>

<ul>
<li>M of size n x n</li>
<li>M[u][v] = 1 if (u,v) is an edge of graph G and M[u][v] = 0 otherwise. For undirected graphs, M[u][v] = 1 implies M[v][u] = 1.</li>
</ul>
<strong>Adjacency lists</strong>

<ul>
<li>An array A of size n; A[u] points to the list of vertices incident to vertex u.</li>
<li>For directed graphs, the adjacency list of vertex u contains the vertices of the outgoing edges.</li>
<li>For undirected graphs, edge (u,v) has u in v’s list and v in u’s list.</li>
<li>Vertices do not necessarily have to be in the sorted order in the list</li>
</ul>
For all problems:

<ul>
<li>If the running time is given, your report needs to explain how it is achieved by your implementation.</li>
<li>If the running time is not given, give the worst-case time bound your implementation achieves along with a brief implementation in the report.</li>
<li>You can use an auxiliary array of size n if needed. Give a brief explanation what it is used for in the report.</li>
<li>The graphs may or may not be connected.</li>
<li>The graphs are always simple</li>
</ul>
<ol>
<li>File IO and Graph representation.</li>
</ol>
<h2>ListGraph</h2>
Implement a ListGraph class. The class should contain a read(String filepath) function and a readWeighted(String filepath) function. These functions will read the graph from the input file and then store it in an adjacency list representation.

You have to come up with your own linked list and write your own node class. Imports are not allowed. The node class should be inside the same file as ListGraph.

public static ListGraph read(String filepath) throws IOException {}

This function reads the unweighted graph stored at the given file path into memory.

vertices are indexed from 0 to . The𝑛lines of the file are indexed starting from 1, ● Line 1 of the file contains a single integer specifying the number of vertices. The as in IntelliJ. 𝑛 − 1

<ul>
<li>For each integer such thatof the file is a space-separated ● For undirected graphs, if an&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; then&nbsp;&nbsp;&nbsp; will be present on line&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; , and</li>
</ul>
list of all vertices 𝑢𝑣 such that&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 𝑢 − 𝑣&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; the𝑢 𝑣graph.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 𝑢

will also be present on line&nbsp;&nbsp; .

<ul>
<li>If𝑢 vertex 𝑢 has no outgoing edges,𝑣 line 2 + 𝑢 will be empty.</li>
</ul>
public static ListGraph readWeighted(String filepath) throws IOException {} This function reads the weighted graph stored at the given file path into memory. The file specification is identical to the unweighted case, except:

<ul>
<li>Line 2 is now a space-separated list of integers specifying the weights of vertices ●&nbsp;&nbsp;&nbsp; The vertices𝑛 − in1 the out-neighbourhood of vertex 𝑢 are now specified on line 3 + 𝑢.</li>
</ul>
through&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; , respectively.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 𝑛&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0

<h2>MatrixGraph</h2>
Implement a MatrixGraph class. This class should contain a read(String filepath) function. This function will read the graph from the input file and then store it in an adjacency matrix representation.

public static MatrixGraph read(String filepath) throws IOException {}

This function reads the unweighted graph stored at the given file path into memory. The file specification is identical to the ListGraph.read case except that it uses the matrix representation to store the graph in place of the list.

<h1>1.&nbsp;&nbsp; Undirected Graph Properties</h1>
<h2>Tree-check</h2>
G is an undirected n-vertex graph represented by adjacency lists. Determine in O(n) time whether G is a tree. public static boolean treeCheck(ListGraph a)

<h2>Counting triangles</h2>
G is an undirected n-vertex graph represented by an adjacency matrix. Count the number of distinct triangles in G in O(n<sup>3</sup>) time. Vertices x, y, and z form a triangle if the edges (x,y), (y, z), and (z,x) are in G. Note: triangle(x,y,z) = triangle(z,x,y). public static int countTriangles(MatrixGraph a)

<h2>Clustering coefficient of a vertex</h2>
G is an undirected n-vertex graph represented by adjacency lists. Given a vertex u, determine u’s clustering coefficient. The clustering coefficient is defined below.

Assume an edge between vertices u and v means that u and v are friends. The clustering coefficient of u is the fraction of pairs of friends of u that are friends with each other. If a vertex has k friends, the clustering coefficient is 0 when none of the k friends are friends with each other; it is 1 when all k friends are friends with each other (i.e., they form a complete graph on k vertices).

More formally, when vertex u has degree d(u), the clustering coefficient of u is 2×(𝑛𝑢𝑚𝑏𝑒𝑟 𝑜𝑓 𝑛𝑒𝑖𝑔ℎ𝑏𝑜𝑟𝑠(𝑑(𝑢 𝑥)× 𝑎𝑛𝑑(𝑑( 𝑢𝑦) 𝑜𝑓−1 𝑢) 𝑤𝑖𝑡ℎ 𝑒𝑑𝑔𝑒 (𝑥,𝑦) 𝑖𝑛 𝐸)

The graph shown below gives the clustering coefficient for each vertex. Vertex A has 4 neighbors. Four vertices can have at most <sup>4</sup>C<sub>2 </sub>= 6 edges between them. For vertex A, 3 pairs of neighbors are friends with each other. A’s clustering coefficient is thus 3/6 = 0.5.

Compute the clustering coefficient of a vertex u in O(n<sup>2</sup>) time. As noted above, you can use an auxiliary array of size n during the computation. You are not supposed to convert the adjacency list representation of the graph into its adjacency matrix representation. public static double vertexClusterCoeff(ListGraph a, int u)

<h2>Clustering coefficient of G</h2>
The global clustering coefficient of a graph is defined as the average of the n clustering coefficients of its vertices. Compute in O(n<sup>3</sup>) time.

public static double graphClusterCoeff(ListGraph a

<h1>2.&nbsp;&nbsp; Directed Graph Properties</h1>
<h2>Compute in-degrees</h2>
G is an n-vertex directed graph represented by adjacency lists. Determine in O(n+m) time the indegrees of all the vertices in the graph. Return an array inDeg where inDeg[u] represents the in-degree of vertex u.

public static int[] computeInDegrees(ListGraph a)

<h2>DAG-check</h2>
G is an n-vertex directed graph represented by adjacency lists. Determine in O(n+m) time whether G is a directed acyclic graph (DAG). If G is a DAG, determine the number of sources and number of sinks.

dagCheck(adjList A) returns a pair of integers (in0, out0), where in0 represents the number of sources and out0 represents the number of sinks. If G is not a DAG, the output should be

(-1,-1).

public static int[] dagCheck(ListGraph a)

<h1>3.&nbsp;&nbsp; Recursive Tree Exploration</h1>
Given is an n-node free tree T=(V,E) with V = {0,1,2,3 …., n-1}. We assume n&gt;2. The tree is represented by adjacency lists. Every node v has a positive integer weight w(v).

You are asked to determine the cost of a <strong>max-weight path P </strong>in tree T which has the following properties:

<ol>
<li>The path P is between two leaves of T.</li>
<li>Selected nodes on path P get marked. The sum of the weights of the marked nodes on P is the weight of the path.</li>
<li>Path P cannot contain two marked nodes that are adjacent. We call a path with no adjacent marked nodes a valid path.</li>
<li>Path P has maximum weight; i.e., the sum of the weights of the marked nodes on P is a maximum over all possible valid paths between any two leaves in T.</li>
</ol>
Consider the tree shown in Figure 1.The green edges between leaves x and y form a valid path as no two marked (green) nodes are adjacent. The cost of the path is 215 and it is a max-weight path.

We note that a path in which marked and unmarked nodes alternate is a valid path. However, in a max-weight path marked and unmarked nodes do not necessarily alternate. This occurs in the path from x to y where the node x is marked and the next two nodes on the max-weight path are not marked. For instance, in Figure 1, this allows the nodes with weights 30 and 35 to be marked, while leaving the two vertices with weight 5 unmarked.

Figure 2 shows three trees that are chains in which the patterns of which nodes are marked vary. The max-weight path does not necessarily alternate nodes and does not need to include the leaf nodes. Note that in a max-weight path there will never be three consecutive unmarked nodes between two marked nodes (as the weights are positive, the middle unmarked node should always be included).

The goal is to find the cost of a max-weight path in T (a tree can contain more than one max-weight path). <strong>The algorithm for finding the cost of a max-weight path needs to have O(n) time complexity and use the recursive formulation described below.</strong>

We describe in section 3.1 a recursive approach for determining which nodes to mark when tree T is a linear chain. In 3.2 we extend the approach to finding the cost of a max-weight path in an arbitrary tree. Make sure you understand the approach for a chain before working on the tree.

<h2>Input Format</h2>
For the input, you will use the method readWeighted(String filepath)you implemented in ListGraph to read in a Graph as a ListGraph containing int []weight indicating the weight of each node weight[i]. You need to implement functions named maxWeightChain, maxWeightTree. The return type should be an integer that is the value of the maximum weighted path.

<h2>3.1.&nbsp; Determining the max-weight in a chain</h2>
Given is a chain C on n nodes represented by adjacency lists. Let s be one of the two leaves of chain C. The max-weight for chain C is computed in O(n) time using the recursive approach described below. Note that you do not need to determine the nodes on the chain contributing to the max-weight.

The chain exploration should start from a leaf node. During recursion, the nodes having a child-parent relationship reflect the recursive calls made (as done in DFS).

Let (u,v) be an edge on the chain. The recursive call made with v as an argument from node u returns three values: in(v), out1(v) and out2(v):

<ul>
<li>in(v): the max-weight achievable when node v is marked (i.e., w(v) is included)</li>
<li>out1(v): the max-weight achievable when node v is not marked and the child of v is marked.</li>
<li>out2(v): the max-weight achievable when neither node v nor the child of v are marked.</li>
</ul>
Node u uses the values of in(v), out1(v) and out2(v) to determine in(u), out1(u) and out2(u). We illustrate this in Figure 3 for one of the chains shown in Figure 2. The triples next to each node represent the three values the node returns.

<ul>
<li>Node f is a leaf and in(f) = w(f) = 100 and the two out-values are 0. Node f returns the triple (100,0,0). This defines the base case of the recursion.</li>
<li>Node e receives (100,0,0) and sets in(e) = w(e) =30 and out1(e) = in(f) =100; out2(e) remains 0. Node e returns the triple (30,100,0).</li>
<li>Work through the triples for nodes d to a on your own and understand what solutions they represent.</li>
<li>Finally, node s receives (415, 310, 400). The quantity 400 represents out2(a), the max-weight achievable in the chain from node a to f that does not include w(a)=15 and w(b)=10. Node s determines its triple to return using the rules stated in Figure 3. The value out2(a) = 400 is used to determine in(s) = 445 = 45+400 which represents the solution marking nodes s, c and f.</li>
</ul>
Let u1 and u2 be the two leaves in the chain. If the initial call is made with leaf u1 then, in(u1) = w(u1), out1(u1) = out2(u1) = 0, and the final returned weight will be max(in(u2),out1(u2)).

Let (u,v) be an edge in the chain. The recursive call made by u receives in(v), out1(v) and out2(v). The three values node u returns are:

<ol>
<li>in(u) = w(u) + max{out1(v), out2(v)}</li>
<li>out1(u) = in(v)</li>
<li>out2(u) = out1(v)</li>
</ol>
When node u is marked, we add to its weight the maximum of the two subsolutions we determined (and return the value in in(u)). When node u is not marked, we return two values reflecting that we either have node v marked (out1(u)) or the second node adjacent to v marked

(out2(u)).

Write function public static int maxWeightChain(ListGraph a) using the recursive approach described above.

<h2>3.2.&nbsp; Determining the max-weight in a tree</h2>
Given a tree T, use a recursive tree exploration approach to determine the cost of the max-weight path in O(n) time. You do not need to find the vertices on the path (there can be more than one such path).

The tree exploration finding the cost of a max-weight path can start at any node s. The final cost returned will be the same for any start node, but some intermediate entries computed at nodes will be different.

The tree exploration has similarities with a DFS exploration on an undirected graph: at node u, all nodes v adjacent to u are considered and a call to v is made if v has not been visited. Make sure you understand the three entries, the call to maxWeightChain returns before reading on.

When the tree exploration starts at a vertex s, the path of max-weight may include node s (see Figure 4(a)). The max weight path can also be between two leaves in a subtree rooted at a node adjacent to the start node. If the start node is node s’, as shown in Figure 4(b), the path is in the subtree rooted at node s (and the path is found in the call made by s’ on s).

This means a recursive call made by node u on its neighbor node v needs to return information about the cost of a path in the subtree rooted at node v (this subtree includes all nodes that are reachable from v through a path that does not pass through u). To correctly compute max-weight, a call returns 4 entries on the subtree explored.

Assume there is an edge from node u to v, and u discovers v. The recursive call from v returns four entries related to the subtree rooted at node v:

<ol>
<li><strong>L2</strong>: max-weight of a path in the subtree rooted at node v. The two end nodes of the path are leaves in the subtree rooted at v. The path can include node v. The cost of this path could be the final max-weight cost of the tree.</li>
<li><strong>in</strong>: max-weight of a path in the subtree rooted at node v from node v to a leaf node. Node v is marked.</li>
<li><strong>out1</strong>: max-weight of a path in the subtree rooted at node v from node v to a leaf node. Node v is not marked. The node adjacent to v on the path is marked.</li>
<li><strong>out2</strong>: max-weight of a path in the subtree rooted at node v from node v to a leaf node. Node v and the node adjacent to v on the path are not marked.</li>
</ol>
Consider the tree shown in Figure 5. The exploration starts at node s and we show the 4-tuple returned by calls to nodes v1, u1, and u2. We show arrows on edges to reflect the calls made.

When we refer to a subtree rooted at a node u we always refer to the tree rooted at node u as the recursive call is made to u. Figure 5 shows the subtree rooted at node v2 shaded assuming v2 is called from s.

In the example tree, node s considers its four adjacent nodes in the order v1, v2, v3, and v4:

<ul>
<li><strong>Node v1 </strong>represents a subtree consisting of the single node v1 having weight 80. It returns (L2, L1.in, L1.out1, L1.out2) = (0, 80, 0, 0). L2=0 as there exists no path between two leaves, marking node v1 results in L1.in=80, and the subtree rooted at v1 contains no other nodes that could contribute to L1.out1 and L1.out2. See Figure 5.</li>
<li><strong>Node v2 </strong>is the root of a subtree containing 10 nodes. Hence, v2 makes two recursive calls: to u1 and u2.</li>
</ul>
○&nbsp;&nbsp;&nbsp; Node u1 returns (L2, L1.in, L1.out1, L1.out2) = (0, 45, 22, 0).

○&nbsp;&nbsp;&nbsp; Node u2 returns (L2, L1.in, L1.out1, L1.out2) = (95, 60, 75, 50).

○&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Node v2 combines these values and returns (L2, L1.in, L1.out1, L1.out2) = (157, 135, 60, 75). The process of combining values returned is described below.

<ul>
<li><strong>Node v3 </strong>makes two recursive calls, each one to a single node subtree. It returns (L2, L1.in, L1.out1, L1.out2) = (37, 10, 22, 0), as shown in Figure 6.</li>
<li><strong>Node v4 </strong>makes two recursive calls and, after combining the two 4-tuples returns (L2, L1.in, L1.out1, L1.out2) = (105, 80, 45, 65).</li>
</ul>
Node s combines the four 4-tuple received from the 4 recursive calls (one 4-tuple from each recursive call). If node s is the root of the tree T and not a leaf, L2(s) is returned as L2(s) is the weight of the max-weighted path. However, when the start node s is a leaf in tree T, max{L2(s), L1.in(s), L1.out1(s)} is returned, which is the cost of the max-weighted path in T.

In Figure 6, we show the other 3 values as well. These values are relevant when the start node s is a leaf in the tree.

We say that u is an ancestor of v (and v is a descendant of u) if u has been called but not returned at the time when v is called. The root of the tree is the ancestor of all other vertices in the tree.

If v has been called from u then u is the parent of v and v is a child of u. This relationship holds only when (u,v) belongs to E.

Naturally, a parent is an ancestor and a child is a descendant.

In the following we sketch how a node u invoking recursive calls on its k children v1, v2, …, vj manages the 4-tuples it receives from each child. There is no need to store all k 4-tuples. As a 4-tuple is received by u, updates to u’s 4-tuple are made.

Before making any call, node u initializes its 4-tuple (L2, L1.in, L1.out1, L1.out2) = (0,0,0,0). Note that when it is clear from the context which node the L-values belong to, we use them as L2, L1.in, etc. If it may not be clear, we use the notation L2(u), L1.in(u) , etc.

Assume node vj returns to u the 4-tuple (L2, L1.in, L1.out1, L1.out2). See Figure 7 for an illustration:

<ul>
<li>L2(vj) is the blue path in the subtree rooted at vj</li>
<li>in(vj) is the black path from a leaf to node vj (vj is marked)</li>
<li>out1(vj) is the red path (red node is marked and vj is not marked)</li>
<li>out2(vj) is the green path (one green node is not marked and one is marked, vj is not marked)</li>
</ul>
<h3>Figure 7</h3>
We describe how node u updates its already determined 4-tuple after receiving the 4-tuple from node vj. Note that the description below uses no additional variables about previously computed entries and hence the order in which entries are updated is important. Do not change the order if you use it in your implementation. If you are making changes, make sure to address all aspects of correctness.

<strong>Updating L2. </strong>Updating L2 means determining the best path between two leaves in the subtree rooted at node u now allowing that the path can go through node u to a leaf in the subtree rooted at vi for i in {1,…,j}.

The new value L2 of u is the maximum of 5 quantities:

L2(u) = max {

<table width="519">
<tbody>
<tr>
<td width="88">L2(u),</td>
<td width="431">previously found best path in the subtree rooted at node u</td>
</tr>
<tr>
<td width="88">L2(vi),</td>
<td width="431">best path in the subtree rooted at node vi</td>
</tr>
</tbody>
</table>
L1.in(u) + max{L1.out1(vi), L1.out2(vi)},

first part of the path going through node u, node u marked, and the second part of the path is in the subtree rooted at vi.

L1.out1(u) + max{L1.in(vi), L1.out1(vi)},

first part of the path going through node u, node u not marked, and the second part of the path is in subtree rooted at vi.

L1.out2(u) + L1.in(vi),

first part of the path going through node u, node u and its

neighbor on that path are not marked, vi is marked, and the second part of the path is in the subtree rooted at vi.

}

<strong>Updating the other three entries of the 4-tuple. </strong>These updates are done after L2(u) has been updated:

<table width="453">
<tbody>
<tr>
<td width="24">●</td>
<td width="96">L1.in(u) =</td>
<td width="333">max {L1.in(u), w(u) + max {L1.out1(vi), L1.out2(vi)}}</td>
</tr>
<tr>
<td width="24">●</td>
<td width="96">L1.out1(u) =</td>
<td width="333">max{ L1.out1(u), L1.in(vi)}</td>
</tr>
<tr>
<td width="24">●</td>
<td width="96">L1.out2(u) =</td>
<td width="333">max {L1.out2(u), L1.out1(vi)}</td>
</tr>
</tbody>
</table>
Try to think why are the entries above being updated as such. Try to think of cases in terms of inclusion and exclusion of the node in the path.

<strong>Base Case:</strong>

The node is a leaf.

For a leaf v , set (L2, L1.in, L1.out1, L1.out2) = (0, w(v), 0, 0).

Write function public static int maxWeightTree(ListGraph a) using the recursive approach described above.

<h1>Project Structure</h1>
You are required to implement the following files:

<ul>
<li>java ● MatrixGraph.java ●&nbsp;&nbsp;&nbsp;&nbsp; UndirectedCheck.java.</li>
<li>java</li>
<li>java</li>
</ul>
ListGraph.java:

You need to implement the following functions:

public static ListGraph read(String filepath) throws IOException {} public static ListGraph readWeighted(String filepath) throws IOException {}

MatrixGraph.java:

You need to implement the following functions:

public static MatrixGraph read(String filepath) throws IOException {}

UndirectedCheck.java:

You need to implement the following functions:

public static boolean treeCheck(ListGraph a) public static int countTriangles(MatrixGraph a) public static double vertexClusterCoeff(ListGraph a, int u) public static double graphClusterCoeff(ListGraph a)

DirectedCheck.java:

You need to implement the following functions: public static int[] computeInDegrees(ListGraph a) public static int[] dagCheck(ListGraph a)

MaxWeight.java:

You need to implement the following functions:

public static int maxWeightChain(ListGraph a) public static int maxWeightTree(ListGraph a)

<h1>Testing your code</h1>
We provide a set of JUnit tests for the functionality in this project at GraphTest.java. Before running the tests, download and extract data.zip from BrightSpace, and change line 14 of GraphTest to point to the extracted directory.

<h1>Report</h1>
You are required to submit a report.

<ul>
<li>The report should describe for each problem in sections 1 and 2 the approach you used and how the stated time complexity is achieved. The description given for each problem should be brief and not repeat material covered in class.</li>
<li>For the two problems in section 3 describe any variations you made to the given description. Clearly address why your code achieves O(n) time.</li>
<li>The final paragraph of the report should address two questions:</li>
</ul>
○&nbsp;&nbsp;&nbsp; Which of the problems was the most interesting? Address why.

○&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Which of the problems was the most challenging one to complete? Address why.

The overall report guidelines and expectations are:

<ul>
<li>The report needs to be typed (use LaTeX or Word).</li>
<li>Your name (Last, First), your Purdue email, and your section number (LE1@4:30 or LE2@1:30) need to be on top of page 1.</li>
<li>The RC statement needs to be given for each problem in section 1, 2 and 3. It should be the first line(s) before the description.</li>
<li>The suggested length of the report is up to 2 pages, with font size 12 and 1.5 spacing. If you have additional supporting material you can include it as an Appendix (which has no page limit). However, only your report will be graded. The appendix may be consulted by the grader for additional information.</li>
<li>Reports are uploaded to Gradescope and code is uploaded to Vocareum.</li>
</ul>
<h1>Grading</h1>
The expected grading rubric is given below. ●&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Coding part (85 points)

○&nbsp;&nbsp;&nbsp; Tree-check, Counting triangles, Clustering coefficient (vertex and graph), in-degrees, DAG-check. (30 Points)

○&nbsp;&nbsp;&nbsp; Recursive exploration on a tree: max-weight on a chain; max-weight on an arbitrary tree (55 Points)

<ul>
<li>Overall quality of the report (15 points)</li>
</ul>
■&nbsp;&nbsp;&nbsp; Quality and conciseness of writing

■&nbsp;&nbsp;&nbsp; Logical flow of arguments for each problem

■&nbsp;&nbsp;&nbsp; Clear explanation of running times your code achieves for each of the eight problems

<h1>Submission</h1>
<ul>
<li>To Vocareum (everything should be inside the src folder):
<ul>
<li>Java</li>
</ul>
</li>
</ul>
○&nbsp;&nbsp;&nbsp; UndirectedCheck.Java

○&nbsp;&nbsp;&nbsp; MaxWeight.Java

○ ListGraph.Java ○ MatrixGraph.Java

<ul>
<li>To Gradescope:
<ul>
<li>pdf</li>
</ul>
</li>
</ul>
<strong>Note</strong>:

<ul>
<li>Additional imports are not allowed. (other than the ones in the starter code)</li>
<li>No other file uploads are allowed. Only those files will be compiled. If you have to write a new Java Class, please do so in one of the files above.</li>
<li>If for some reason you do not see the src folder under the work folder on Vocareum, please make a new src folder.</li>
<li>This has been explained on Piazza already so you can refer to it there. ● Please go to office hours for additional help.</li>
</ul>
