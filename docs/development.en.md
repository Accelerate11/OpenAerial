# Development

[中文](development.md) | [English](development.en.md)

The repository currently contains directory structure, brand assets, and documentation templates. There is no common build or runtime entry point yet.

## Toolchain records

Each design or software module documents in its README:

- Tool names, exact versions, and supported operating systems.
- Required design libraries, symbols, footprints, or software dependencies.
- Steps to open, build, export, or run it.
- Expected results and known limitations.

Product-level build, installation, and flashing instructions belong in the product's `docs/deployment.md`. CAD tools, flight firmware, and middleware are not prescribed at platform level.

## File management

Use UTF-8 for text. Root `.gitattributes` defines line ending conventions.

Maintain Chinese `.md` and sibling English `.en.md` documentation with language links. Designs, code, and machine-readable manifests share one source; original records retain their original language.

Version design sources and necessary exports. Consider Git LFS for large or frequently changing binary design files after confirming contributors can retrieve complete files.

Index raw datasets, weights, and large runtime logs in [Resources](../resources/README.en.md). Keep build output, caches, and local environment files out of source history.

## Checks

Add checks when content requires them: designs open with complete references, electronics include necessary libraries, BOMs match assemblies, software builds, and parameters match hardware revisions.

Put automation with defined inputs and acceptance criteria in `tools/`; put product-specific validation in its `tests/`.
