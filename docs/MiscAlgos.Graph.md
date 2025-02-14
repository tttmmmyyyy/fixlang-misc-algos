# `module MiscAlgos.Graph`

# Types and aliases

## `namespace MiscAlgos.Graph`

### `type Edge c = unbox struct { ...fields... }`

#### field `from : Std::I64`

#### field `to : Std::I64`

#### field `cost : c`

### `type Graph c = unbox struct { ...fields... }`

#### field `edges : Std::Array (Std::Array (MiscAlgos.Graph::Edge c))`

#### field `size : Std::I64`

### `type NodeDistance c = unbox struct { ...fields... }`

The pair of a node and a distance.

#### field `node : Std::I64`

#### field `dist : c`

# Traits and aliases

# Trait implementations

### `impl [c : Std::LessThan] MiscAlgos.Graph::NodeDistance c : Std::LessThan`

# Values

## `namespace MiscAlgos.Graph::Graph`

### `add_bidirectional_edge : Std::I64 -> Std::I64 -> c -> MiscAlgos.Graph::Graph c -> MiscAlgos.Graph::Graph c`

Add an bidirectional edge.

### `add_edge : Std::I64 -> Std::I64 -> c -> MiscAlgos.Graph::Graph c -> MiscAlgos.Graph::Graph c`

Add an edge.

The first argument is the starting node, the second is the ending node,
and the third is the cost of the edge.

### `dijkstra : [c : Std::Additive, c : Std::LessThan, c : Std::LessThanOrEq] Std::I64 -> c -> MiscAlgos.Graph::Graph c -> Std::Array c`

Given a graph and a starting node, returns an array of costs to reach each node from the starting node.

The second argument is the value to represent infinity.

### `make_discrete : Std::I64 -> MiscAlgos.Graph::Graph c`

Create a graph with the given number of nodes.

## `namespace MiscAlgos.Graph::NodeDistance`

### `make : Std::I64 -> c -> MiscAlgos.Graph::NodeDistance c`