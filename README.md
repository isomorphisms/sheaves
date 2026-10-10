# sheaves

FAC and onward.

This repository has two purposes:

1. keep concise reading notes and source maps for the development of sheaf theory;
2. extract a small "rising sea" foundation suitable for Idriç: shapes, patches, sections, restriction, gluing, and tensor-compatible local structure.

The goal is not to reproduce textbooks. It is to isolate the reusable logic and make its laws explicit enough to become types.

## Start here

- [`books/`](books/README.md) — summaries and public-source map for Vakil, FAC, Tôhoku, and Stacks.
- [`idric/rising-sea-foundations.md`](idric/rising-sea-foundations.md) — the proposed type-level core.

The first implementation target is deliberately below schemes and cohomology:

```text
shape
  → patch
  → section
  → restriction
  → overlap / compatibility
  → gluing
  → local scalars and modules
  → tensor-compatible restriction
  → affine/quasicoherent localization
```

A public reading link is not treated as permission to republish a source. Full mirrors belong here only when redistribution terms are clear.
