# Contributing

[中文](CONTRIBUTING.md) | [English](CONTRIBUTING.en.md)

Thank you for contributing to OpenAerial. The repository is establishing development documentation for OpenAerial 150; product designs and code have not yet been released.

## File placement

- Product-specific materials belong in `products/<product-id>/`.
- Original modules actually reused by multiple products belong in `shared/`, with their consumers documented.
- Shared tools belong in `tools/`; platform rules belong in `docs/`.
- Sources, fixed versions, download locations, and checksums for large resources belong in `resources/`.

Use stable lowercase English directory names with hyphens. Display names may include spaces: OpenAerial 150 uses the directory `openaerial-150`.

## What to document in a contribution

1. The affected product or shared module and the purpose of the change.
2. Changes to mechanical design, electronics, BOMs, parameters, software, or documentation.
3. Design tools, exact versions, libraries, and other dependencies.
4. Checks performed, results, and aspects that remain unverified.
5. Origins, attribution, and applicable licenses. Preserve third-party notices.

Mechanical and electronic design submissions include editable sources and corresponding exports from the same revision. Update configurations, BOMs, documentation, and sources together.

## Validation and change records

Record product validation in its `tests/` directory. Add changes to the product's Unreleased changelog section and mark unverified capabilities as pending validation.

Before a release, follow the [release process](docs/releases.en.md) to confirm compatible versions and reproduction materials.

## Chinese and English

Maintain documentation as sibling files: the default `.md` is Chinese and `.en.md` is English. Place language links below the title. Update both versions together, keeping specifications, status, and validation scope aligned.

Code, CAD files, BOMs, wiring tables, and configurations share one source. Preserve original records and generation prompts in their original language; both documentation versions link to that source.
