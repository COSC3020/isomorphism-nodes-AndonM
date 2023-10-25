[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11974290&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Assume that graphs A & B are isomorphic in spite of their differing node count. Let $n_{1}$ be the number of nodes in A, and $n_{2}$ be the number of nodes in B. Assume that $n_{1}$ < $n_{2}$. Under the assumption that A and B are isomorphic, all vertices u and v in A, uv is an edge in A iff f(u)f(v) is an edge in B. Consider the node u in A that is not in the range of f (there isn't a corresponding node for u in B). This is possible because A and B have a differenet number of nodes, and if they were isomorpic, every node in A would have a corresponding node in B. Since u has no corresponding node in B, there are no edges incident to u in A. However, in B, there must be a corresponding node f(u), and it should be connected to some other nodes since graph B is isomorphic to A. That means there has to be at least one edge incident to f(u) in B. This creates a contradiction as the edge(s) incident to u in A does not have a corresponding edge(s) in B, and the edge(s) incident to f(u) in B does not have a corresponding edge(s) in A. This contradiction shows that the assumption that A and B are isomorphic cannot be true; thus proving that if A and B do not have the same amount of nodes, they cannot be isomorphic.
