# 食品数据库分发中心 · Food Catalog Releases

本仓库用于分发独立版本的食品成分与包装商品数据库，包括 SQLite 数据文件、版本清单、校验信息和来源许可说明。数据构建与审校在独立流程中进行，两个数据库的发布和更新互不影响。

Public distribution of independently versioned food composition and packaged-product datasets. Each release channel has its own database, manifest, provenance, and licence notices.

## 数据库 / Catalogs

| 数据集 | 内容 | Release | 状态 |
| --- | --- | --- | --- |
| **BLS 4.0 中文食品成分库** / BLS 4.0 Chinese Food Composition | 基础食材、烹饪状态、宏量及微量营养成分；支持中文名称 | [`bls-foods-stable`](https://github.com/Xleia/bls4-zh-catalog/releases/tag/bls-foods-stable) | 已发布 |
| **日本 OFF 包装食品目录** / Japan Open Food Facts | 日本地区的条码商品，重点改进全家、7-Eleven、罗森的覆盖率和营养信息质量 | `off-foods-jp-stable` | 构建与审核中，尚未发布 |

## 分发方式 / Distribution

- 每个数据集使用**独立 Release Tag**；更新日本 OFF 不会更改 BLS 的发布内容。
- 数据库文件名称、Manifest 结构和版本字段遵循既有使用方的兼容契约。下载和导入前应验证文件哈希与数据库结构。
- 未通过数据来源、营养单位、许可和差异校验的构建版本不会发布到稳定通道。
- 此仓库只负责**公开数据分发**；不托管原始大规模导出、人工审校草稿或私有构建工作流。

## 数据来源与许可 / Sources and licences

**BLS 4.0**：德国 Max Rubner-Institut 的食品成分数据；请以 BLS Release 随附的来源和许可文件为准。

**Open Food Facts（OFF）**：日本商品目录基于 [Open Food Facts](https://world.openfoodfacts.org/) 数据，数据库衍生作品遵守 [Open Database License 1.0（ODbL）](https://opendatacommons.org/licenses/odbl/1-0/) 的适用要求。图片及其他第三方材料可能适用不同许可。未获核实许可的零售商数据不纳入公开包。

营养值需明确每 100g / 100ml 与每包装的区别；不得把未核实重量的整包营养数据误写成每 100g 数据。

## Releases

- [查看所有数据库版本 / All releases](https://github.com/Xleia/bls4-zh-catalog/releases)
- [BLS 4.0 稳定通道 / BLS stable](https://github.com/Xleia/bls4-zh-catalog/releases/tag/bls-foods-stable)

日本 OFF 稳定通道只有在首版数据完成验证后才会创建，现阶段没有可下载的正式 OFF 数据包。
