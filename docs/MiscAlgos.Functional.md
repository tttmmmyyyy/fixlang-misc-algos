# MiscAlgos.Functional

Defined in misc-algos@0.7.2

A module that gathers useful functions for functional programming.

## Values

### namespace MiscAlgos.Functional::Tuple2

#### diagonal

Type: `a -> (a, a)`

Creates a tuple with the same element.

#### map0

Type: `(a -> c) -> (a, b) -> (c, b)`

Maps a function over the first element of a tuple.

#### map01

Type: `(a -> b) -> (a, a) -> (b, b)`

Maps a function over both elements of a tuple.

#### map1

Type: `(b -> c) -> (a, b) -> (a, c)`

Maps a function over the second element of a tuple.

#### swap

Type: `(a, b) -> (b, a)`

Swaps the elements of a tuple.

### namespace MiscAlgos.Functional::Tuple3

#### diagonal

Type: `a -> (a, a, a)`

Creates a tuple with the same element.

#### map0

Type: `(a -> d) -> (a, b, c) -> (d, b, c)`

Maps a function over the first element of a tuple.

#### map012

Type: `(a -> b) -> (a, a, a) -> (b, b, b)`

Maps a function over all elements of a tuple.

#### map1

Type: `(b -> d) -> (a, b, c) -> (a, d, c)`

Maps a function over the second element of a tuple.

#### map2

Type: `(c -> d) -> (a, b, c) -> (a, b, d)`

Maps a function over the third element of a tuple.

## Types and aliases

## Traits and aliases

## Trait implementations