# lambda-cube

I'm too lazy to texify this right now.  Maximally "featureful" types for each calculus.  I've elide the foralls. int(x) is the singleton type for a given x; list(x) is a list of length x.  Really, lists are recursive and so require more powerful calculi, but I needed an example for a dependent tycon.

## Non-dependent calculi

### λ→ (STLC with some primitive type)
f: int → int

### λK (STLC with tycons)
f: int lsit → int list

### λ∀ (STLC with polymorphism)
f: ɑ → ɑ

### F (STLC with polymorphism and tycons)
f: ɑ list → ɑ list

## Dependent (Π) calculi

### λΠ (Dependent STLC with some primitive type)
f: Πx: int. int(x) → int(x)

### λΠK (Dependent STLC with tycons)
f: f: Πx:int. int list(x) → int list(x)

### λΠ∀ (Dependent STLC with polymorphism)
f: Πx: int. ɑ → int(x) // weird

### CoC (Dependent STLC with polymorphism and tycons)
f: Πx: int. ɑ list(x) → ɑ list(x)
