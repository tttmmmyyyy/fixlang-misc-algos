# `module MiscAlgos`

Miscellaneous algorithms.

# Types and aliases

## `namespace MiscAlgos`

### `type P1000000007 = unbox struct { ...fields... }`

### `type ZP p = unbox struct { ...fields... }`

Finaite field Z/pZ.

#### field `value : Std::U32`

#### field `prime : p`

# Traits and aliases

## `namespace MiscAlgos`

### `trait a : FromU32`

#### method `from_U32 : Std::U32 -> a`

### `trait p : PrimeProvider`

#### method `create : p`

#### method `value : p -> Std::U32`

# Trait implementations

### `impl MiscAlgos::P1000000007 : MiscAlgos::PrimeProvider`

### `impl [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p : MiscAlgos::FromU32`

### `impl [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p : Std::Add`

### `impl [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p : Std::Div`

### `impl [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p : Std::Eq`

### `impl [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p : Std::Mul`

### `impl [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p : Std::Neg`

### `impl [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p : Std::Sub`

### `impl Std::I64 : MiscAlgos::FromU32`

# Values

## `namespace MiscAlgos`

### `binom_table : [r : MiscAlgos::Ring] Std::I64 -> Std::Array (Std::Array r)`

Creates table for binomial coefficients.
`binom_table(m).@(n).@(k)` is binom(n, k) for 0 <= k <= n < m.

### `binomial_by_facts : [r : MiscAlgos::Ring, r : Std::Div] Std::I64 -> Std::I64 -> Std::Array r -> r`

`binomial_by_facts(n, k, fact)` calculates `n! / (k! * (n-k)!)` using a factorial table `fact`.

### `factorial_table : [r : MiscAlgos::Ring] Std::I64 -> Std::Array r`

`factorial_table(n)` returns an array of `n!` for 0 <= i < n.

### `monomials_by_facts : [r : MiscAlgos::Ring, r : Std::Div] Std::I64 -> Std::I64 -> Std::Array r -> r`

`monomials_by_facts(n, k, fact)` calculates the number of monomials of degree `n` with `k` variables using a factorial table `fact`.

## `namespace MiscAlgos::FromU32`

### `from_U32 : [a : MiscAlgos::FromU32] Std::U32 -> a`

## `namespace MiscAlgos::PrimeProvider`

### `create : [p : MiscAlgos::PrimeProvider] p`

### `value : [p : MiscAlgos::PrimeProvider] p -> Std::U32`

## `namespace MiscAlgos::ZP`

### `inv : [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p -> MiscAlgos::ZP p`

### `power : [p : MiscAlgos::PrimeProvider] Std::U32 -> MiscAlgos::ZP p -> MiscAlgos::ZP p`