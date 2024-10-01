# `module MiscAlgos`

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

### `binomial_by_fact : [r : MiscAlgos::Ring, r : Std::Div] Std::I64 -> Std::I64 -> Std::Array r -> r`

`binomial_by_fact(n, k, fact)` calculates `n! / (k! * (n-k)!)` using a factorial table `fact`.

### `factorial_table : [r : MiscAlgos::Ring] Std::I64 -> Std::Array r`

`factorial_table(n)` returns an array of `n!` for 0 <= i < n.

### `fold_rep : Std::I64 -> a -> (Std::I64 -> a -> a) -> a`

`fold_rep(n, state, body)` calculates `state.body(0).body(1)....body(n-1)`.

When `n <= 0`, it returns `state` as is.

### `fold_rep_rev : Std::I64 -> a -> (Std::I64 -> a -> a) -> a`

`fold_rep_rev(n, state, body)` calculates `state.body(n-1).body(n-2)....body(0)`.

When `n <= 0`, it returns `state` as is.

### `loop_rep : Std::I64 -> a -> (Std::I64 -> a -> Std::LoopResult a a) -> a`

TODO: move this to `Std`?

## `namespace MiscAlgos::FromU32`

### `from_U32 : [a : MiscAlgos::FromU32] Std::U32 -> a`

## `namespace MiscAlgos::PrimeProvider`

### `create : [p : MiscAlgos::PrimeProvider] p`

### `value : [p : MiscAlgos::PrimeProvider] p -> Std::U32`

## `namespace MiscAlgos::ZP`

### `@prime : MiscAlgos::ZP p -> p`

Retrieves the field `prime` from a value of `ZP`.

### `@value : MiscAlgos::ZP p -> Std::U32`

Retrieves the field `value` from a value of `ZP`.

### `act_prime : [f : Std::Functor] (p -> f p) -> MiscAlgos::ZP p -> f (MiscAlgos::ZP p)`

Updates a value of `ZP` by applying a functorial action to field `prime`.

### `act_value : [f : Std::Functor] (Std::U32 -> f Std::U32) -> MiscAlgos::ZP p -> f (MiscAlgos::ZP p)`

Updates a value of `ZP` by applying a functorial action to field `value`.

### `inv : [p : MiscAlgos::PrimeProvider] MiscAlgos::ZP p -> MiscAlgos::ZP p`

### `mod_prime : (p -> p) -> MiscAlgos::ZP p -> MiscAlgos::ZP p`

Updates a value of `ZP` by applying a function to field `prime`.

### `mod_value : (Std::U32 -> Std::U32) -> MiscAlgos::ZP p -> MiscAlgos::ZP p`

Updates a value of `ZP` by applying a function to field `value`.

### `power : [p : MiscAlgos::PrimeProvider] Std::U32 -> MiscAlgos::ZP p -> MiscAlgos::ZP p`

### `set_prime : p -> MiscAlgos::ZP p -> MiscAlgos::ZP p`

Updates a value of `ZP` by setting field `prime` to a specified one.

### `set_value : Std::U32 -> MiscAlgos::ZP p -> MiscAlgos::ZP p`

Updates a value of `ZP` by setting field `value` to a specified one.