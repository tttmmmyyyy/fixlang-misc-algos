# `module MiscAlgos.ZP`

Miscellaneous algorithms.

# Types and aliases

## `namespace MiscAlgos.ZP`

### `type P1000000007 = unbox struct { ...fields... }`

### `type ZP p = unbox struct { ...fields... }`

Finaite field Z/pZ.

#### field `value : Std::U32`

#### field `prime : p`

# Traits and aliases

## `namespace MiscAlgos.ZP`

### `trait p : PrimeProvider`

#### method `create : p`

#### method `value : p -> Std::U32`

# Trait implementations

### `impl MiscAlgos.ZP::P1000000007 : MiscAlgos.ZP::PrimeProvider`

### `impl [p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : MiscAlgos.Traits::FromU32`

### `impl [p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Add`

### `impl [p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Div`

### `impl [p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Eq`

### `impl [p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Mul`

### `impl [p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Neg`

### `impl [p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p : Std::Sub`

# Values

## `namespace MiscAlgos.ZP::PrimeProvider`

### `create : [p : MiscAlgos.ZP::PrimeProvider] p`

### `value : [p : MiscAlgos.ZP::PrimeProvider] p -> Std::U32`

## `namespace MiscAlgos.ZP::ZP`

### `inv : [p : MiscAlgos.ZP::PrimeProvider] MiscAlgos.ZP::ZP p -> MiscAlgos.ZP::ZP p`

### `power : [p : MiscAlgos.ZP::PrimeProvider] Std::U32 -> MiscAlgos.ZP::ZP p -> MiscAlgos.ZP::ZP p`