# 整机 BOM

[中文](README.md) | [English](README.en.md)

[bom.csv](bom.csv) 已记录市售 MicoAir743 飞控，数量 1 为整机规划用量；硬件修订待核对。电调型号与数量确认后补入 BOM，当前尚无完整整机物料清单。

## 字段

| 字段 | 用途 |
| --- | --- |
| item_id | 稳定条目标识，与图纸、装配及替代关系对应 |
| parent_id | 上级装配条目标识；顶层物料可留空 |
| category | 物料分类，随实际物料统一约定 |
| name | 物料名称 |
| part_number | 自研零件或产品内部编号 |
| revision | 适用设计修订 |
| quantity | 整机或所属装配需要的数量 |
| unit | 数量单位 |
| manufacturer | 制造商 |
| manufacturer_part_number | 制造商型号或料号 |
| source_url | 采购或官方资料来源 |
| alternative_item_ids | 已评估替代条目标识，多个值用分号分隔 |
| notes | 装配、兼容性及其他备注 |

CSV 使用 UTF-8。物料名称或备注包含逗号时使用标准 CSV 引号。

每次物料变更核对装配关系、供电、接口、配置与验证范围。替代件经评估后再列为兼容选项；价格估算如后续加入，应记录币种、来源和日期。
