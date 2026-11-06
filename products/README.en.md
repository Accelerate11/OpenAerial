# Product workspaces

[中文](README.md) | [English](README.en.md)

Each product uses a stable directory name containing design, manufacturing, software, and validation materials.

The first product is [OpenAerial 150](openaerial-150/README.en.md), identified by `openaerial-150`.

## Adding a product

1. Create `<product-id>/` using lowercase English letters, numbers, and hyphens.
2. Follow the applicable OpenAerial 150 organization, documenting the new product's designs, parameters, and validation independently.
3. Describe its name, purpose, status, specifications, and reproduction entry points.
4. Create its system BOM, changelog, and release manifest.
5. Update the root product table.

Leave undefined technical modules marked pending. Document modules that do not apply to the product.

## Maturity

- Planning: requirements, specifications, and approach are being defined.
- In design: design or implementation materials are being developed.
- Prototype validation: a prototype exists and validation results are being recorded.
- Reproducible release: compatible versions, public reproduction materials, and validation scope are documented.

Optional product configurations belong in its `configs/`. Extract original modules to `shared/` when multiple products actually reuse them.
