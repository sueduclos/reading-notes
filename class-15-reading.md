[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 15: DSA: Trees

### Common terminology for a binary tree:

-   `root` - The first or starting `Node` of the tree. Everything branches from this `Node`
-   `left` - The **left child** is the `Node` to the left of a parent `Node`
-   `right` - The **right child** is the `Node` to the right of a parent `Node`
-   **edge** - An edge is a connection between two `Nodes`. In code, this is not really phyically represented, it's just a representation of the references between a parent `Node` and the child `Node`.
-   **leaf** - A leaf `Node` is a `Node` without any subsequent edges / connections
-   **height** - The height of a tree is the number of `Node` "levels" it has, usually counted via the number of edges from top to bottom. 
                                               

### Vocabulary
| Term                    | Definition |
| ----------------------- | ---------- |
| tree                    |            |
| binary tree             |            |
| root                    |            |
| parent                  |            |
| child                   |            |
| edge                    |            |
| height                  |            |
| left child              |            |
| right child             |            |
| Depth-First Traversal   |            |
| Breadth-First Traversal |            |
| recursion               |            |
| binary search tree      |            |
| k-ary tree              |            |

### Discussion Questions:

#### 1.What is a leaf node? Why is it important to be able to find leaf nodes? 
A leaf `Node` is a `Node` without any subsequent edges / connections. It's the end of part of the tree.

#### 2. Describe the differences between pre-order, in-order, and post-order traversal. Why are they called pre,  in, and post order? 
**Pre-order** means that the root has to be looked at first
The biggest difference between each of the traversals is when you are looking at the root node.
pre-order : pre-order output of tree nodes
in-order: in-order output of tree nodes
post-order: post-order output of tree nodes

#### 3. What is the height of a fully balanced (each non-leaf node has two children) tree? What is this used for? 
A “perfect” binary tree is one where every non-leaf node has exactly two children. The maximum width for a perfect binary tree, is 2^(h-1), where h is the height of the tree. Height can be calculated as log n, where n is the number of nodes.

#### 4. How are stacks and queues used in relation to trees? 
TBD
