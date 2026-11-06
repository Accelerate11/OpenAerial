# OpenAerial 150

[中文](README.md) | [English](README.en.md)

OpenAerial 的第一款产品，按机械结构、电子硬件、固件、软件、训练、仿真和验证资料组织完整工作目录。

**当前状态：规划中，尚未发布。** 当前文件是研发资料模板；产品设计、运行代码与测试结果尚待补充。

## 产品定义

| 项目 | 当前内容 |
| --- | --- |
| 产品名称 | OpenAerial 150 |
| 产品标识 | `openaerial-150` |
| 用途与目标用户 | 待定义 |
| 构型与尺寸 | 待定义 |
| 重量、载荷与动力 | 待定义 |
| 飞控 | 市售 MicoAir743，硬件修订与固件版本待补充 |
| 电调 | 市售成品模块，具体型号待补充 |
| 计算与传感器 | 待选型 |
| 工作环境与运行条件 | 待定义 |
| 已验证能力 | 暂无验证记录 |

“150”为当前产品名称的一部分，其具体规格含义待定义。

## 工作目录

| 目录 | 资料范围 |
| --- | --- |
| [mechanical](mechanical/README.md) | 可编辑结构设计、导出文件与工程图 |
| [electronics](electronics/README.md) | 市售飞控、电调的选型、供电和接线资料 |
| [bom](bom/README.md) | 整机物料、采购来源和替代件 |
| [firmware](firmware/README.md) | 固件来源、烧录、准确版本与必要补丁 |
| [software](software/README.md) | 机载程序、驱动、自主能力与应用 |
| [learning](learning/README.md) | 数据处理、训练、评估与模型配置 |
| [simulation](simulation/README.md) | 仿真模型、场景与任务 |
| [configs](configs/README.md) | 实际产品配置、参数与标定示例 |
| [tests](tests/README.md) | 台架、仿真与实机验证 |

## 复现流程

1. 查阅 [BOM](bom/bom.csv)，核对设计修订和实际配置。
2. 按[装配说明](docs/assembly.md)完成制造、装配和接线。
3. 按[标定说明](docs/calibration.md)记录标定结果。
4. 按[部署说明](docs/deployment.md)安装匹配版本。
5. 按[操作说明](docs/operation.md)执行已定义的验证流程。
6. 遇到问题时查阅[故障排查](docs/troubleshooting.md)。

以上文档当前均为待填写模板。

## 版本、资源与许可

- [发布清单](release.yaml)：软硬件配套关系，当前为草稿。
- [变更记录](CHANGELOG.md)：本产品的未发布变更与后续版本。
- [大型资源索引](../../resources/README.md)：数据集、权重与大型日志。
- [许可说明](../../docs/licensing.md)：自研资产的许可尚待确定。
