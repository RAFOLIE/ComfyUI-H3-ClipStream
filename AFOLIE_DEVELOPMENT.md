# 来源与后续开发说明

本开发副本基于 [AraneaQwQ/ComfyUI-H3-ClipStream](https://github.com/AraneaQwQ/ComfyUI-H3-ClipStream)，后续由 [RAFOLIE](https://github.com/RAFOLIE) 维护自己的修改。

- 直接上游维护者：AraneaQwQ；完整贡献历史保留在 Git 中。
- 初始基线：`2718be5d78567eea5d8fa17e9a29fb4aefae8da3`。
- 原项目还集成 NikoDemon80 的 Motion-Context 和 knoic 的 PrefixStream Clip Bin；原有 [ATTRIBUTION.md](ATTRIBUTION.md) 完整保留。
- 保留 [GPLv3 LICENSE](LICENSE) 及原有版权声明。分发修改版本时遵循适用的 GPLv3 条款，提供对应源码、保留声明并明确标注修改及日期；不能仅用本来源说明替代许可要求。
- 本副本的修改不代表原作者发布或背书；原作者及集成组件作者均应获得其工作的署名。

## 修改记录

- 2026-09-28：补充本说明及 README 来源入口。初始准备阶段仅添加来源说明，随后实施的迁移见下列记录。

后续在此记录功能修改、兼容性变化和验证结果，发布前更新到实际状态。

- 2026-09-28：将 10 个活动节点迁移到 ComfyUI V3（ComfyNode、define_schema、类方法 execute、NodeOutput、ComfyExtension）；保留节点 ID、输入名及输出顺序。
- 2026-09-28：适配 Nodes 2.0 的 DOM 控件尺寸与生命周期，移除卡片刷新时的自动缩小；改用包内导入。迁移测试见 [V3_MIGRATION.md](V3_MIGRATION.md)。

- 2026-09-28：增大新建节点默认尺寸（MiniMax H3 Dual Clip Picker：680 × 640），仅在创建时应用；加载工作流保留已保存尺寸，用户仍可手动缩放。

- 2026-09-28：整理 V3 与 Nodes 2.0 开发版，安装地址改为 RAFOLIE/ComfyUI-H3-ClipStream；保留原作者来源、许可证及 Git 历史。
