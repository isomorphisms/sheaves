# Ravi Vakil — *The Rising Sea: Foundations of Algebraic Geometry*

## Why this is the primary working reference

Vakil is unusually good for the specific layer wanted here: he repeatedly moves
between abstract sheaf language and the affine calculation that explains it.

For this repository, the important chain is

```text
patch
  → sections on a patch
  → restriction to a smaller patch
  → compatible local sections
  → gluing
  → sheaves of rings/modules
  → quasicoherent sheaves
  → localization on distinguished affine patches
  → tensor product
```

The aim is not to encode schemes wholesale. It is to understand which parts of
that chain are generic local-to-global structure and which parts depend on
commutative algebra.

## The key affine calculation

If

```text
U = Spec A
V = D(f) = Spec A_f
```

and a quasicoherent sheaf `F` corresponds on `U` to an `A`-module `M`,
then restriction to `V` is localization:

```text
sections F U       ≅ M
sections F V       ≅ M_f
restrict U→V       ≅ M → M_f
```

This is the computational content worth preserving in a type system.
Restriction is not an arbitrary callback: for this kind of local object it has
a canonical algebraic realization.

## Tensor

For quasicoherent `F` and `G` on an affine patch,

```text
sections (F ⊗ G) (Spec A) ≅
sections F (Spec A) ⊗_A sections G (Spec A)
```

and after restricting to `D(f)`,

```text
(M ⊗_A N)_f ≅ M_f ⊗_(A_f) N_f.
```

That compatibility is stronger than the bare definition of a sheaf. It should
therefore live in a stronger Idriç interface rather than being silently assumed
for every local family.

## What Idriç should steal

Not the notation `Spec` or the whole scheme hierarchy. Steal:

- patch inclusion as typed evidence;
- sections indexed by their patch;
- restriction whose source and target patches occur in the type;
- identity and composition laws for restriction;
- overlap/meet of patches;
- compatibility and gluing;
- a separate algebraic layer where scalar restriction and tensor commute;
- a still stronger affine/quasicoherent layer where restriction is
  localization.

## Public source

Vakil's author page links the public notes:

https://math.stanford.edu/~vakil/

A 2024 public draft containing the quasicoherent restriction/localization and
tensor discussion is:

https://math.stanford.edu/~vakil/216blog/FOAGfeb1724public.pdf

Do not mirror the book text here without explicit redistribution permission.
