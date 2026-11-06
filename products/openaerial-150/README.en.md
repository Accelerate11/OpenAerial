# OpenAerial 150

[中文](README.md) | [English](README.en.md)

The first OpenAerial product, organized around mechanical design, electronics, firmware, software, learning, simulation, and validation.

**Status: planning; not released.** These are development documentation templates. Product designs, runnable code, and test results are still to be added.

## Product definition

| Item | Current status |
| --- | --- |
| Name | OpenAerial 150 |
| Identifier | `openaerial-150` |
| Purpose and target users | To be defined |
| Configuration and dimensions | To be defined |
| Weight, payload and propulsion | To be defined |
| Flight controller | Commercial MicoAir743; hardware revision and installed firmware pending |
| ESC | Commercial module; exact model pending |
| Compute platform and sensors | To be selected |
| Environment and operating conditions | To be defined |
| Validated capabilities | No validation records |

“150” is part of the current product name; its specification meaning remains to be defined.

## Workspace

| Directory | Contents |
| --- | --- |
| [mechanical](mechanical/README.en.md) | Editable designs, exports, and engineering drawings |
| [electronics](electronics/README.en.md) | Commercial flight controller and ESC selection, power, and wiring |
| [bom](bom/README.en.md) | System parts, sources, and alternatives |
| [firmware](firmware/README.en.md) | Firmware sources, flashing, exact versions, and patches |
| [software](software/README.en.md) | Onboard programs, drivers, autonomy, and applications |
| [learning](learning/README.en.md) | Data processing, training, evaluation, and model configuration |
| [simulation](simulation/README.en.md) | Models, environments, and tasks |
| [configs](configs/README.en.md) | Actual hardware configurations, parameters, and calibration examples |
| [tests](tests/README.en.md) | Bench, simulation, and hardware validation |

## Reproduction workflow

1. Review the [BOM](bom/bom.csv) and matching design revisions and configuration.
2. Follow [assembly](docs/assembly.en.md) for manufacturing, assembly, and wiring.
3. Follow [calibration](docs/calibration.en.md) and record results.
4. Install matching versions using [deployment](docs/deployment.en.md).
5. Follow [operation](docs/operation.en.md) and the defined validation procedures.
6. Consult [troubleshooting](docs/troubleshooting.en.md) when needed.

These guides are currently unfilled templates.

## Versions, resources, and licensing

- [Release manifest](release.yaml): compatible hardware and software, currently a draft.
- [Changelog](CHANGELOG.en.md): unreleased changes and future versions.
- [Resources](../../resources/README.en.md): datasets, weights, and large logs.
- [Licensing](../../docs/licensing.en.md): licenses for original assets remain pending.
