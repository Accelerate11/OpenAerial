# Architecture and organization

[中文](architecture.md) | [English](architecture.en.md)

This document defines how materials are organized. Each product records its actual component choices and open documentation scope. OpenAerial 150 uses a commercial MicoAir743 flight controller and an off-the-shelf ESC. The ESC model, firmware, middleware, compute platform, sensors, and algorithms remain to be specified.

## Product boundaries

A product directory describes a system that can be understood, assembled, and validated independently. Mechanical design, electronics, the system BOM, firmware, software, configuration, simulation, and operating guides together form its reproduction materials.

The product's `release.yaml` records the compatible hardware and software combination for a release. The current file is a draft.

## Shared module boundaries

Extract an original module to `shared/` when multiple products actually need it and its interface can be documented independently. Products record exact dependencies, required configuration, and compatibility.

Reference upstream projects through their origin, fixed version or commit, and local patches. Document how modifications differ from upstream.

## Configurations and product generations

Optional configurations belong in the product's `configs/<configuration-id>/`, with matching BOMs, software, and validation results. No configurations have been defined yet.

Evaluate a separate product directory when structures, interfaces, or assembly methods change substantially. Track mechanical revisions, board revisions, software versions, and system releases separately.

## Material flow

Editable design → exported and manufacturing files → BOM and assembly → deployment and calibration → simulation or hardware validation → fixed release.

When a change affects this flow, update the relevant materials and preserve their provenance and version relationships.

## Commercial modules and original hardware

Record commercial component selection, sources, installation, power, wiring, and integration validation in the product's `electronics/` directory. Reference manufacturer designs within their actual published scope.

Create `source/` and `fabrication/` for original boards when design work begins. Clearly distinguish project-authored designs and integration materials from external modules and their official documentation.
