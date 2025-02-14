# `module MiscAlgos.Geometry`

# Types and aliases

## `namespace MiscAlgos.Geometry`

### `type Vec2 = unbox struct { ...fields... }`

#### field `x : Std::F64`

#### field `y : Std::F64`

# Traits and aliases

# Trait implementations

### `impl MiscAlgos.Geometry::Vec2 : Std::Add`

### `impl MiscAlgos.Geometry::Vec2 : Std::Eq`

### `impl MiscAlgos.Geometry::Vec2 : Std::Neg`

### `impl MiscAlgos.Geometry::Vec2 : Std::Sub`

# Values

## `namespace MiscAlgos.Geometry::Vec2`

### `distance : MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2 -> Std::F64`

### `dot : MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2 -> Std::F64`

### `length : MiscAlgos.Geometry::Vec2 -> Std::F64`

### `make : Std::F64 -> Std::F64 -> MiscAlgos.Geometry::Vec2`

### `scaled : Std::F64 -> MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2`

### `to_tuple : MiscAlgos.Geometry::Vec2 -> (Std::F64, Std::F64)`