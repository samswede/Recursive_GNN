
# Recursive Graph Neural Networks (Recursive_GNN)

## Why

In a world of rapidly evolving data structures and interconnected systems, traditional flat or singly-nested graph models often fall short in capturing the true complexity of real-world data. Hierarchical structures and dependencies, a common feature in many domains including biology, social networks, manufacturing processes, and more, cannot be accurately captured by these conventional approaches. Recursive_GNN emerges as a solution to this challenge by offering a flexible and versatile tool that models and embeds arbitrarily nested graphs, making it capable of capturing complex, hierarchical systems with unprecedented precision.

## How

Recursive_GNN works by employing a novel recursive approach that computes embeddings for nodes in a graph and its sub-graphs. The algorithm is initialized by assigning random embeddings to the nodes. Then, for each node, if it has a nested graph, the same computation is performed on the nested graph recursively. The current node's embedding and the aggregate embedding of the nested graph (if present) are then combined to form the final embedding for the node. The recursion unravels the nested graph hierarchy, ensuring that all levels of complexity are addressed and captured in the final model.

## What

This repository contains the implementation of Recursive_GNN. Here's a breakdown of the contents:

1. `recursive_gnn.py`: The core implementation of the Recursive_GNN algorithm.

2. `utils.py`: Utility functions used for data loading, preprocessing, and post-processing.

3. `node_functions.py`: Different node function implementations that can be used with Recursive_GNN.

4. `combine_functions.py`: Different combine function implementations that can be used with Recursive_GNN.

5. `aggregate_functions.py`: Different aggregate function implementations that can be used with Recursive_GNN.

6. `examples/`: Example usage of Recursive_GNN on various datasets.

7. `tests/`: Unit tests to ensure the correctness of the implementation.

## Getting Started

To use Recursive_GNN, follow these steps:

1. Clone the repository
```
git clone https://github.com/username/Recursive_GNN.git
```

2. Navigate to the cloned repository
```
cd Recursive_GNN
```

3. Install the necessary requirements
```
pip install -r requirements.txt
```

4. Run the examples
```
python examples/example.py
```

We invite researchers and developers to explore this repository, use Recursive_GNN in their projects, and join us in improving and expanding its capabilities.

```
