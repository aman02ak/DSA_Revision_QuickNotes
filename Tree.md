# TREE
## Binary Tree: 
Def: A binary tree is a tree data structure with nodes having atmost 2 children.

- Maximum number of nodes in a Binary Tree at level `'l' = (2^l)`
    - For root node, level `l = 0`

- Maximum number of nodes in a Binary Tree of height `'h' = (2^h - 1)`
    - total_nodes = (2^0) + (2^1) + (2^2) + ... + (2^l); `h = l + 1`
    - total_nodes = 1 * (1 - 2^h) / (1 - 2); `Geometric Progression`
    - total_nodes = (2^h - 1); `Hence Proved`
- Minimum possible height of a Binary Tree with `N` Nodes = `logBase2(N + 1)`
- Minimum possible levels of a Binary Tree with `m` Nodes = `|logBase2(m)| + 1`

### Full Binary Tree
Def: A binary tree in which every node has 0 or 2 children.

### Complete Binary Tree
Def: A binary tree with all levels completely filled except the last one, and last level has all keys as left as possible.

### Perfect Binary Tree
Def: A binary tree with all internal nodes have 2 childrens and all leaf nodes are at same level.
- Perfect Binary Tree with height `h` has `(2^h - 1)` nodes.
- Number of leaf nodes = `(I + 1)`; `I: Number of Internal Nodes`

### Balanced Binary Tree
Def: A binary tree with height, `h = (log(n))`; where n is number of nodes in binary tree.

### Degenerate/Pathological Binary Tree
Def: A tree where every internal nodes has one child.
- Performance wise it is same as Linked List.

## Handshaking Lemma
Def: It is about undirected graph. 

- In every undirected graph, number of Odd Degreee Vertices will always be even.
- As per this Handshaking Lemma, degree sum formula = `SUM(deg(v)) = 2 * |E|`
- i.e. Sum of degree of vertices will always be even and equals to `SUM(deg(v)) = 2 * |E|`
- A tree is a unidirectional acyclic Graph
- In a tree where every node has either 0 or K childrens, following properties is always true.
    - `L = (K - 1) * I + 1`; `L: # of Leaf Nodes`; `I: # of Internal Nodes`
- In a binary tree, number of leaf nodes is always one more than nodes with 2 children.
    - `L = T + 1`; `T: # of Internal nodes with 2 Child`

Note: A Binary Tree with nodes having no labels are Unlabelled Binary Tree.
- Number of different Unlabelled Binary Tree with `n` nodes = `Catalan Number` = `SUM(T(i) * T(n-i-1))`
- Or, `T(n) = (2n)! / [(n + 1)! * n!]`
- Number of Binary Search Tree(BST) with n nodes = `# of Unlabelled Binary Trees = Catalan Number`
- Number of labelled Binary Tree = `(# of Unlabelled Binary Trees) * n!` = `(2n)! / (n + 1)!`
    - Reason for this is like for every unlablled tree with n Nodes can create n! different labelled trees.