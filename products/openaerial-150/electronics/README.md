# 电子硬件

[中文](README.md) | [English](README.en.md)

OpenAerial 150 当前采用市售飞控和电调。飞控已确定为 MicoAir743；电调的品牌、型号和数量尚待补充。本目录维护模块选型、官方资料、安装接口、供电和接线等系统集成资料。

```text
electronics/
├── README.md
├── flight-controller/  MicoAir743 的选型与集成资料
├── esc/                成品电调，具体型号待补充
└── wiring/             整机供电、线束与接口连接记录
```

[飞控资料](flight-controller/README.md)、[电调资料](esc/README.md)与[接线记录](wiring/README.md)分别维护；采购物料进入[整机 BOM](../bom/bom.csv)，装配步骤进入[装配说明](../docs/assembly.md)。

本产品目前没有自研板卡。外购模块的原厂原理图、PCB 和制造资料按厂商实际公开范围引用；本项目记录自研设计与集成资料各自的来源和许可。

未来如新增自研板卡，再为实际板卡建立 `custom-boards/<board-id>/source/` 与 `fabrication/`，保存可编辑设计和对应制造文件。
