# De Bruijn Graphs

Let's say you have a very, very small circular genome. It's sequence is ATGGCGTGCA, but you don't know that yet. 

![This is your \(very small\) genome of interest. But we don&apos;t know that yet.](../../.gitbook/assets/image%20%286%29.png)

Since we don't know the whole genome, we do some sequencing and end up getting the following reads:  
CGTGCAA, ATGGCGT, CAATGGC, GGCGTGC, and TGCAATG. Of course, we could align these reads by hand but, in a real-world example, we would have many, many too many reads to align by hand.   
  
If were to align these reads by hand, however, and walk over the aligned sequences \(like an ant walking along the overlapping reads\) we would follow this bolded path: **AT**GGCGT → **GG**CGTGC → **CG**TGCAA → **TG**CAATG → **CA**ATGGC → **AT**GGCGT. This sort of walk is called a hamiltonian cycle \(where we go to one node exactly once\).   
  
We can make a graph so that it clearly has a hamiltonian cycle like this: \(1\) Get all of the kmers, like **ATGGCGT** and make these nodes of a graph \(2\) call the prefix of the kmer **ATGGCG**T and the suffix A**TGGCGT** and make these edges ****\(3\) Connect one k-mer to another if the suffix of one kmer equals the prefix of another. So, for example, **GGCGTG**C and T**GGCGTG** have a prefix and suffix that match so, for example T**GGCGTG  -&gt; GGCGTG**C, so we can represent this as a node **T** that travels along the **GGCGTG** edge to get to the node **C**. But, as we get more reads, making a graph like this gets really difficult. There's no known efficiency algorithm to find a Hamiltonian cycle in a large graph \(in fact, it's one of the big problems that computer scientists struggle to solve\).   
  
In the Hamiltonian graph problem, we were trying to visit every node of the graph once. But, there are efficient algorithms to visit every \*edge\* in the graph once. So instead of assigning each k-mer to a node, we will now assign each k-mer located within a read to an edge. This allows the construction of a de Bruijn graph. To make that graph, first make a node for every _unique_ prefix or suffix in a k-mer. So if you have the reads ATTTA and ATTTG, make just one node with the sequence ATTT. Then, if you have two reads-- x and y--where x's prefix is the node and y's suffix is the node, you can connect the prefix from y with the suffix from x. It'll look something like this: 

![A De Bruijn graph](../../.gitbook/assets/image%20%2810%29.png)

Now, our problem is to visit every edge in that De Bruijn graph. And, luckily, this \*does\* have an efficient algorithm. It was solved by the famous mathematician Euler when he was trying to figure out how to cross 7 bridges in a city without crossing any bridge twice. The sort of cycle where you cross every edge just once is thus called an Eulerican cycle. He proved that a connected graph with undirected edges contains an Eulerian cycle exactly when every node in the graph has an even number of edges touching it.  
  
Basically, to traverse this graph, you just keep crossing edges until you have no more edges to cross. Take an analogy where you put an ant on the graph and tell it to randomly explore the graph under a single constraint: the ant cannot traverse a previously traversed edge. Sooner or later, the ant must get stuck at a certain node \(with all outgoing edges previously traversed\) and, at that point, you've found an Eulerian cycle. It's a little more complicated than that, so read the paper linked below for more info, but that's the gist.   
  
This example was taken basically directly from this paper:

{% embed url="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5531759/pdf/nihms329513.pdf" %}



  
  


