# Stacks Project — Sheaves of Modules

## Role in this repository

Use the Stacks Project as the modern definition and lemma checker.

Vakil is the preferred first explanation. FAC and Tôhoku give historical
motivation. Stacks is where we verify that a proposed law is actually true at
the stated level of generality.

## Relevant ladder

The current *Sheaves of Modules* chapter contains, in useful order:

- sections of sheaves of modules;
- quasi-coherent modules;
- coherent modules;
- locally free sheaves;
- bilinear maps;
- tensor product;
- flat modules;
- duals;
- internal Hom;
- invertible modules;
- localization.

That order is a good warning against collapsing everything into one type.

## Tensor subtlety

For arbitrary sheaves of modules, the naive rule

```text
U ↦ F(U) ⊗_(O(U)) G(U)
```

does not by itself give the final sheaf in full generality. Tensor product is a
sheaf-level construction (equivalently, the relevant presheaf construction is
sheafified).

By contrast, on the distinguished affine basis for quasicoherent sheaves the
module calculation behaves cleanly:

```text
(M ⊗_A N)_f ≅ M_f ⊗_(A_f) N_f.
```

The Idriç interfaces must preserve that distinction.

## Source

Browse:

https://stacks.math.columbia.edu/browse

Current Sheaves of Modules PDF:

https://stacks.math.columbia.edu/download/modules.pdf

Tôhoku bibliography entry, including Stacks tags that explicitly use the paper:

https://stacks.math.columbia.edu/bibliography/Tohoku

The Stacks Project is licensed for redistribution under its own stated terms;
if source is mirrored later, preserve its license and provenance rather than
copying isolated text without the surrounding license.
