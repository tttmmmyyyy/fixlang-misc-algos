# MiscAlgos.Combinatorics

Defined in misc-algos@0.7.2

## Values

### namespace MiscAlgos.Combinatorics

#### binom_table

Type: `[r : MiscAlgos.Traits::Ring] Std::I64 -> Std::Array (Std::Array r)`

Creates table for binomial coefficients.
`binom_table(m).@(n).@(k)` is binom(n, k) for 0 <= k <= n < m.

#### binomial_by_facts

Type: `[r : MiscAlgos.Traits::Ring, r : Std::Div] Std::I64 -> Std::I64 -> Std::Array r -> r`

`binomial_by_facts(n, k, fact)` calculates `n! / (k! * (n-k)!)` using a factorial table `fact`.

#### factorial_table

Type: `[r : MiscAlgos.Traits::Ring] Std::I64 -> Std::Array r`

`factorial_table(n)` returns an array of `n!` for 0 <= i < n.

#### monomials_by_facts

Type: `[r : MiscAlgos.Traits::Ring, r : Std::Div] Std::I64 -> Std::I64 -> Std::Array r -> r`

`monomials_by_facts(n, k, fact)` calculates the number of monomials of degree `n` with `k` variables using a factorial table `fact`.

## Types and aliases

## Traits and aliases

## Trait implementations