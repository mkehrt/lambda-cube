# lambda-cube

Maximally "featureful" types for each calculus.  I've elided the foralls and added a primitive type `int` and a tycon `list`. `int(x)` is the singleton type for a given `x`; `list(x)` is a list of length `x`.  Really, lists are recursive and so require more powerful calculi, but I needed an example for a dependent tycon.

## Non-dependent calculi

### λ→ (STLC)
f: int → int

### λK (STLC with tycons)
f: int list → int list

### λ∀ (STLC with polymorphism)
f: ɑ → ɑ

### F (STLC with polymorphism and tycons)
f: ɑ list → ɑ list

## Dependent (Π) calculi

### λΠ (Dependent STLC)
f: Πx: int. int(x) → int(x)

### λΠK (Dependent STLC with tycons)
f: Πx:int. int list(x) → int list(x)

### λΠ∀ (Dependent STLC with polymorphism)
f: Πx: int. ɑ → int(x) // weird

### CoC (Dependent STLC with polymorphism and tycons)
f: Πx: int. ɑ list(x) → ɑ list(x)
