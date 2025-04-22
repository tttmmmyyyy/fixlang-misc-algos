# MiscAlgos.ZP

Defined in misc-algos@0.7.2

Miscellaneous algorithms.

## Values

### namespace MiscAlgos.ZP::PrimeProvider

#### create

Type: `[p : MiscAlgos.ZP::PrimeProvider] p`

#### value

Type: `[p : MiscAlgos.ZP::PrimeProvider] p -> Std::U32`

### namespace MiscAlgos.ZP::ZP

#### inv

Type: `[p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p -> MiscAlgos.ZP::ZP p`

#### power

Type: `[p : MiscAlgos.ZP::PrimeProvider] Std::U32 -> MiscAlgos.ZP::ZP p -> MiscAlgos.ZP::ZP p`

## Types and aliases

### namespace MiscAlgos.ZP

#### P1000000007

Defined as: `type P1000000007 = unbox struct { ...fields... }`

#### ZP

Defined as: `type ZP p = unbox struct { ...fields... }`

Finaite field Z/pZ.

##### field `value`

Type: `Std::U32`

##### field `prime`

Type: `p`

## Traits and aliases

### namespace MiscAlgos.ZP

#### trait `p : PrimeProvider`

##### method `create`

Type: `p`

##### method `value`

Type: `p -> Std::U32`

## Trait implementations

### impl `MiscAlgos.ZP::P1000000007 : MiscAlgos.ZP::PrimeProvider`

### impl `[p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : MiscAlgos.Traits::FromU32`

### impl `[p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Add`

### impl `[p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Div`

### impl `[p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Eq`

### impl `[p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Mul`

### impl `[p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Neg`

### impl `[p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Sub`