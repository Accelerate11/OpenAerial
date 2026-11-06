# System bill of materials

[中文](README.md) | [English](README.en.md)

[bom.csv](bom.csv) records the commercial MicoAir743 flight controller. One board is the planned quantity; its hardware revision needs verification. Add the ESC after its model and quantity are confirmed. The system BOM is not complete yet.

## Fields

| Field | Purpose |
| --- | --- |
| item_id | Stable entry identifier used by drawings, assembly, and alternatives |
| parent_id | Parent assembly identifier; blank for a top-level part |
| category | Part classification, standardized as actual parts are added |
| name | Part name |
| part_number | Original part number or internal identifier |
| revision | Applicable design revision |
| quantity | Quantity per system or parent assembly |
| unit | Quantity unit |
| manufacturer | Manufacturer |
| manufacturer_part_number | Manufacturer model or part number |
| source_url | Purchasing or official documentation source |
| alternative_item_ids | Evaluated alternatives, separated by semicolons |
| notes | Assembly, compatibility, and other notes |

Use UTF-8 and standard CSV quoting for commas in names or notes.

When parts change, review assembly, power, interfaces, configuration, and validation scope. List alternatives as compatible only after evaluation. If cost estimates are added, record currency, source, and date.
