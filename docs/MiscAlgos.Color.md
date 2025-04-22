# MiscAlgos.Color

Defined in misc-algos@0.7.2

## Values

### namespace MiscAlgos.Color

#### height_to_rgb

Type: `Std::F64 -> Std::F64 -> (Std::F64, Std::F64, Std::F64)`

Represents a positive real number by a color.

The first argument is the value to be represented, and the second argument is the maximum value.
Zero is represented by red, and the maximum value is represented by blue.

The output is a tuple of (Red, Green, Blue) in the range [0, 1].

#### hsv_to_rgb

Type: `(Std::F64, Std::F64, Std::F64) -> (Std::F64, Std::F64, Std::F64)`

Convert HSV to RGB.

The input is a tuple of (Hue, Saturation, Value) in the range [0, 1].
The output is a tuple of (Red, Green, Blue) in the range [0, 1].

#### rgb_to_hsv

Type: `(Std::F64, Std::F64, Std::F64) -> (Std::F64, Std::F64, Std::F64)`

Convert RGB to HSV.

The input is a tuple of (Red, Green, Blue) in the range [0, 1].
The output is a tuple of (Hue, Saturation, Value) in the range [0, 1].

## Types and aliases

## Traits and aliases

## Trait implementations