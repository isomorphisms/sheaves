# Jean-Pierre Serre — *Faisceaux algébriques cohérents* (FAC, 1955)

## Why it matters here

FAC is useful less as a source of modern notation than as a demonstration of
the move we want Idriç to understand:

> algebraic information is not one global object; it is information carried on
> patches, related by restriction, with finiteness/coherence conditions that
> make local algebra control global geometry.

The paper begins with general sheaf operations before specializing them to
algebraic geometry. That is exactly the separation this repository should keep:
first the local-to-global calculus, then stronger geometric/algebraic
structures.

## Concepts to extract

### Sections and restriction

A sheaf carries data over each admissible region and maps it to data over a
smaller region. The region is part of the meaning of the value. In code, a
section over `U` should therefore not have the same unindexed type as a section
over `V`.

### Local algebra

Once the sheaf carries modules, kernels, cokernels, tensor products and related
algebraic constructions can themselves be considered locally.

The important implementation lesson is not "add every operation from FAC".
It is that the algebraic object should remain tied to the patch over which its
scalars and sections make sense.

### Coherence

Coherence is a finiteness condition stable enough under local algebra to make
the category useful. It belongs above the minimal sheaf interface. Idriç should
first know what restriction and gluing mean; coherent modules can then refine
that structure.

## Historical place

FAC predates Grothendieck's scheme language. It should therefore be read here as
evidence that the fundamental abstraction is genuinely the local-to-global
one, not `Scheme` as a primitive compiler concept.

## Public reading copies

A complete recent AI-assisted French/English working edition and comparison
materials are publicly readable on Zenodo:

https://zenodo.org/records/22074486

Miles Reid's FAC course page also indexes FAC, an English translation, and
course notes:

https://mreid.warwick.ac.uk/MA940/

These are links, not a claim that every linked file may be redistributed from
this repository.
