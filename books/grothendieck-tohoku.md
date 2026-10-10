# Alexandre Grothendieck — *Sur quelques points d'algèbre homologique* (Tôhoku, 1957)

## Why it matters here

Tôhoku is not mainly needed to define `patch` or `restrict`. Its lesson for
this project is architectural: once the right categorical structure has been
identified, constructions that looked specific to sheaves become instances of
general algebra.

Grothendieck's introduction explicitly starts from the formal analogy between
sheaf cohomology and derived functors for modules and seeks a common framework.
That is a useful model for Idriç: encode the smallest laws that make many
apparently unrelated constructions instances of the same operation.

## Concepts to extract later

- abelian categories;
- kernels and cokernels at the categorical level;
- exactness;
- injective objects;
- left exact functors and derived functors;
- Grothendieck's AB conditions;
- sheaf cohomology as an instance rather than a language special case.

These should **not** be prerequisites for the first rising-sea layer. The first
layer should compile useful patch/restriction programs without importing
homological algebra.

## Relation to the sheaf core

The progression we want is:

```text
shape / patch
  ↓
sections / restriction / gluing
  ↓
ringed and module-valued local data
  ↓
abelian structure where available
  ↓
derived constructions
```

This keeps Tôhoku's abstraction available without making every local object
pretend to be an abelian category.

## Public sources

The original paper is free access at J-STAGE:

https://www.jstage.jst.go.jp/article/tmj1949/9/2/9_2_119/_article

The Centre for Grothendieckian Studies bibliographic page:

https://csg.igrothendieck.org/published-works/

A current French/English machine-readable production is publicly available on
Zenodo; the 2026 production line is indexed under the title
"Alexandre Grothendieck — Sur quelques points d'algèbre homologique (Tôhoku):
French and English editions".

As with FAC, public access is not automatically treated as permission to copy
the entire work into this repository.
