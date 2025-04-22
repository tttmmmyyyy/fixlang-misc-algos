# MiscAlgos.Geometry

Defined in misc-algos@0.7.2

## Values

### namespace MiscAlgos.Geometry::Rectangle

#### @pos

Type: `MiscAlgos.Geometry::Rectangle -> MiscAlgos.Geometry::Vec2`

#### @size

Type: `MiscAlgos.Geometry::Rectangle -> MiscAlgos.Geometry::Vec2`

#### from_pos_size

Type: `MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Rectangle`

#### make

Type: `Std::F64 -> Std::F64 -> Std::F64 -> Std::F64 -> MiscAlgos.Geometry::Rectangle`

### namespace MiscAlgos.Geometry::Vec2

#### @length

Type: `MiscAlgos.Geometry::Vec2 -> Std::F64`

#### angle

Type: `MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2 -> Std::F64`

Calculates the angle between two vectors.

`angle(v, w)` returns the rotation angle in radians that rotates the vector `v` to the vector `w`.

##### Parameters

* `v` - The first vector.
* `w` - The second vector.

#### distance

Type: `MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2 -> Std::F64`

#### dot

Type: `MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2 -> Std::F64`

#### hadamard

Type: `MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2`

Calculate the Hadamard product of two vectors, i.e., element-wise multiplication.

#### make

Type: `Std::F64 -> Std::F64 -> MiscAlgos.Geometry::Vec2`

#### make_from_tuple

Type: `(Std::F64, Std::F64) -> MiscAlgos.Geometry::Vec2`

#### rotated

Type: `Std::F64 -> MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2`

Rotate a vector by an angle.

#### scaled

Type: `Std::F64 -> MiscAlgos.Geometry::Vec2 -> MiscAlgos.Geometry::Vec2`

#### to_tuple

Type: `MiscAlgos.Geometry::Vec2 -> (Std::F64, Std::F64)`

## Types and aliases

### namespace MiscAlgos.Geometry

#### Rectangle

Defined as: `type Rectangle = unbox struct { ...fields... }`

##### field `x`

Type: `Std::F64`

##### field `y`

Type: `Std::F64`

##### field `w`

Type: `Std::F64`

##### field `h`

Type: `Std::F64`

#### Vec2

Defined as: `type Vec2 = unbox struct { ...fields... }`

##### field `x`

Type: `Std::F64`

##### field `y`

Type: `Std::F64`

## Traits and aliases

## Trait implementations

### impl `MiscAlgos.Geometry::Vec2 : Std::Add`

### impl `MiscAlgos.Geometry::Vec2 : Std::Eq`

### impl `MiscAlgos.Geometry::Vec2 : Std::Neg`

### impl `MiscAlgos.Geometry::Vec2 : Std::Sub`