# MiscAlgos.Graph

Defined in misc-algos@0.7.2

## Values

### namespace MiscAlgos.Graph::Graph

#### add_bidirectional_edge

Type: `Std::I64 -> Std::I64 -> c -> MiscAlgos.Graph::Graph c -> MiscAlgos.Graph::Graph c`

Add an bidirectional edge.

#### add_edge

Type: `Std::I64 -> Std::I64 -> c -> MiscAlgos.Graph::Graph c -> MiscAlgos.Graph::Graph c`

Add an edge.

The first argument is the starting node, the second is the ending node,
and the third is the cost of the edge.

#### dijkstra

Type: `[c : Std::Additive, c : Std::LessThan, c : Std::LessThanOrEq] Std::I64 -> c -> MiscAlgos.Graph::Graph c -> Std::Array c`

Given a graph and a starting node, returns an array of costs to reach each node from the starting node.

The second argument is the value to represent infinity.

#### make_discrete

Type: `Std::I64 -> MiscAlgos.Graph::Graph c`

Create a graph with the given number of nodes.

### namespace MiscAlgos.Graph::NodeDistance

#### make

Type: `Std::I64 -> c -> MiscAlgos.Graph::NodeDistance c`

## Types and aliases

### namespace MiscAlgos.Graph

#### Edge

Defined as: `type Edge c = unbox struct { ...fields... }`

##### field `from`

Type: `Std::I64`

##### field `to`

Type: `Std::I64`

##### field `cost`

Type: `c`

#### Graph

Defined as: `type Graph c = unbox struct { ...fields... }`

##### field `edges`

Type: `Std::Array (Std::Array (MiscAlgos.Graph::Edge c))`

Edges in the graph.
Edges from node i to another are stored in edges.@(i).

##### field `size`

Type: `Std::I64`

The number of nodes in the graph.

#### NodeDistance

Defined as: `type NodeDistance c = unbox struct { ...fields... }`

The pair of a node and a distance.

##### field `node`

Type: `Std::I64`

##### field `dist`

Type: `c`

## Traits and aliases

## Trait implementations

### impl `[c : Std::LessThan] MiscAlgos.Graph::NodeDistance c : Std::LessThan`