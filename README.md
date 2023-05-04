Download Link: https://assignmentchef.com/product/solved-csci-3104-problem-set-8
<br>
<ol>

 <li>(10 pts) Ginerva Weasley is playing with the network given below. Help her calculate the number of paths from node 1 to node 14.</li>

</ol>

Hint: assume a “path” must have at least one edge in it to be well defined, and use dynamic programming to fill in a table that counts number of paths from each node <em>j </em>to 14, starting from 14 down to 1.

<ol start="2">

 <li>(10 pts) Ginny Weasley needs your help with her wizardly homework. She’s trying to come up with an example of a directed graph <em>G </em>= (<em>V,E</em>), a start vertex <em>v </em>∈ <em>V </em>and a set of tree edges <em>E<sub>T </sub></em>⊆ <em>E </em>such that for each vertex <em>v </em>∈ <em>V </em>, the unique path in the graph (<em>V,E<sub>T</sub></em>) from <em>s </em>to <em>v </em>is a shortest path in <em>G</em>, yet the set of edges <em>E<sub>T </sub></em>cannot be produced by running a depth-first search on <em>G</em>, no matter how the vertices are ordered in each adjacency list. Include an explanation of why your example satisfies the requirements.</li>

 <li>(15 pts) Prof. Dumbledore needs your help to compute the in- and out-degrees of all vertices in a directed multigraph <em>G</em>. However, he is not sure how to represent the graph so that the calculation is most efficient. For each of the three possible representations, express your answers in asymptotic notation (the only notation Dumbledore understands), in terms of <em>V </em>and <em>E</em>, and justify your claim.

  <ul>

   <li>An <em>adjacency matrix </em> Assume the size of the matrix is known.</li>

   <li>An <em>edge list </em> Assume vertices have arbitrary labels.</li>

   <li>An <em>adjacency list </em> Assume the vector’s length is known.</li>

  </ul></li>

 <li>(30 pts) Deep in the heart of the Hogwarts School of Witchcraft and Wizardry, there lies a magical grey parrot that demands that any challenger efficiently convert directed multigraphs into directed <em>simple </em> If the wizard can correctly solve a series of arbitrary instances of this problem, the parrot will unlock a secret passageway.</li>

</ol>

Let <em>G </em>= (<em>E,V </em>) denote a directed multigraph. A directed simple graph is a <em>G</em><sup>0 </sup>= (<em>V,E</em><sup>0</sup>), such that <em>E</em><sup>0 </sup>is derived from the edges in <em>E </em>so that (i) every directed multiedge, e.g., {(<em>u,v</em>)<em>,</em>(<em>u,v</em>)} or even simply {(<em>u,v</em>)}, has been replaced by a single directed

1

<strong>input </strong><em>G </em>= (<em>V,E</em>)                                                <strong>output </strong><em>G</em>′ = (<em>V,E</em>′)

An example of transforming <em>G </em>→ <em>G</em><sup>0</sup>

edge {(<em>u,v</em>)} and (ii) all self-loops (<em>u,u</em>) have been removed.

Describe and analyze an algorithm (explain how it works, give pseudocode if necessary, derive its running time and space usage, and prove its correctness) that takes <em>O</em>(<em>V </em>+ <em>E</em>) time and space to convert <em>G </em>into <em>G</em><sup>0</sup>, and thereby will solve any of the Sphinx’s questions. Assume both <em>G </em>and <em>G</em><sup>0 </sup>are stored as adjacency lists.

Hermione’s hints: Don’t assume adjacencies Adj[u] are ordered in any particular way, and remember that you can add edges to the list and then remove ones you don’t need.

<ol start="5">

 <li>(15 pts extra credit) Professor McGonagall has provided the young wizard Ron with three magical batteries whose sizes are 42, 27, and 16 morts, respectively. (A <em>mort </em>is a unit of wizard energy.) The 27-mort and 16-mort batteries are fully charged (containing 27 and 16 morts of energy, respectively), while the 42-mort battery is empty, with 0 morts. McGonagall says that Ron is only allowed to use, repeatedly, if necessary, the <em>mort transfer spell </em>when working with these batteries. This spell transfers all the morts in one battery to another battery, and it halts the transfer either when the source battery has no morts remaining or when the destination battery is fully charged (whichever comes first).</li>

</ol>

2

McGonagall challenges Ron to determine whether there exists a sequence of morttransfer spells that leaves exactly 12 morts either in the 27-mort or in the 16-mort battery.

<ul>

 <li>Ron knows this is actually a graph problem. Give a precise definition of how tomodel this problem as a graph, and state the specific question about this graph that must be answered.</li>

 <li>What algorithm should Ron apply to solve the graph problem?</li>

 <li>Apply that algorithm to McGonagall’s question. Report and justify your answer.</li>

</ul>

3