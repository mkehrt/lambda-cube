# lambda-cube

I'm too lazy to texify this right now.  Maximally "featureful" types for each calculus.  I've elide the foralls.

## Non-dependent calculi

### λ→ (STLC with some primitive type)
f: int → int

### λK (STLC with tycons)
f: int lsit → int list

### λ∀ (STLC with polymorphism)
f: ɑ → ɑ

### F (STLC with polymorphism and tycons)
f: ɑ list → ɑ option

## Dependent (Π) calculi

### λΠ (Dependent STLC with some primitive type)
f: Πx: int. int(x) → int(x)

### λΠK (Dependent STLC with tycons)
f: f: Πx:int. int list(x) → int list(x)

### λΠ∀ (Dependent STLC with polymorphism)
f: Πx: int. ɑ → int(x) // weird

Π (Dependent STLC with polymorphism and tycons)
f: Πx: int. ɑ list(x) → ɑ list(x)
