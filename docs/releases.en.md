# Product release process

[中文](releases.md) | [English](releases.en.md)

No product has been released yet. This process supports future releases of reproducible product configurations.

## Before releasing

1. Check product specifications, maturity, and validated capabilities.
2. Fix mechanical, board, and system BOM revisions; check source and exported files agree.
3. Fix configurations and dependencies for firmware, software, training, and simulation.
4. Complete assembly, calibration, deployment, operation, and troubleshooting guides.
5. Perform applicable validation and provide concise reports or indexes in the product's `tests/`.
6. Check licensing and attribution, plus locations, versions, and SHA-256 checksums for large resources.
7. Complete `release.yaml` and the product changelog.

List outstanding validation explicitly in the release notes.

## Version naming

Use `<product-id>/v<version>` for system release tags. For example, `openaerial-150/v0.1.0` is a possible future tag, not an existing release.

Maintain mechanical, board, and software revisions separately and record compatibility in the system manifest. Preserve history with Git commits and tags.

## Manifest fields

- `schema_version`: format version, currently 1.
- `product`: stable identifier and display name.
- `release`: version, status, date, and exact source reference using a release tag or fixed commit.
- `hardware`: mechanical revision, original board revisions, purchased modules, and the product-relative BOM path. Each `purchased_modules` entry records its identifier, role, manufacturer, model, revision, quantity, source, and integration documentation path.
- `configurations`: supported configurations with identifiers, directories, and applicable revisions.
- `dependencies`: third-party or shared module names, sources, fixed versions, and patches.
- `artifacts`: deliverable names, locations, SHA-256 checksums, and licenses.
- `validation`: validation status and report references.

Drafts may contain nulls. Complete every applicable field before release and identify anything not applicable. Local paths are relative to the product directory.

## Deliverables

Package designs, manufacturing files, firmware, and other deliverables as needed, with checksums for external files. State applicable configurations, validation scope, and known limitations.
