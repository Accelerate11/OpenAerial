# Electronics

[中文](README.md) | [English](README.en.md)

OpenAerial 150 currently uses commercial flight controllers and ESCs. The flight controller is MicoAir743; the ESC manufacturer, model, and quantity remain pending. This directory records selection, official references, installation interfaces, power, and wiring.

```text
electronics/
├── README.md
├── flight-controller/  MicoAir743 selection and integration
├── esc/                Commercial ESC; exact model pending
└── wiring/             System power, harness and interface records
```

Maintain [flight controller](flight-controller/README.en.md), [ESC](esc/README.en.md), and [wiring](wiring/README.en.md) documentation separately. Add purchased parts to the [system BOM](../bom/bom.csv) and assembly steps to the [assembly guide](../docs/assembly.en.md).

There are no original boards in this product yet. Reference commercial module schematics, PCBs, and manufacturing materials within the manufacturer's actual published scope, recording origins and licenses for project designs and integration materials.

If original boards are developed later, create `custom-boards/<board-id>/source/` and `fabrication/` for editable designs and matching manufacturing files.
