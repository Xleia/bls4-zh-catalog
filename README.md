# Train Libre Food Catalog Releases

公开的 Train Libre 食品数据库分发仓库。构建和审校流程在独立的私有仓库完成；这里仅存放可公开再分发的构建产物、Manifest 和许可说明。

Public distribution repository for independently versioned Train Libre food catalogs. Build and curation workflows are maintained separately.

## Existing release: BLS 4.0 / 中文基础食品库

- **Release tag:** [`bls-foods-stable`](https://github.com/Xleia/bls4-zh-catalog/releases/tag/bls-foods-stable)
- **Artifacts:** `catalog_manifest.json`, `train_libre_base_foods.db.gz`, `THIRD_PARTY_NOTICES.md`
- **Builder:** private `Xleia/train-libre-bls-catalog-zh`
- **Status:** existing production channel; kept unchanged.

## Planned release: Japan Open Food Facts (OFF) / 日本包装食品

- **Reserved release tag:** `off-foods-jp-stable` (**not published yet**)
- **Planned artifacts:** `off_catalog_manifest_jp.json`, `train_libre_off_jp.db`, `off_build_report_jp.json`, `off_diff_report_jp.json`, `off_release_notes_jp.md`, and OFF attribution/license notices
- **Builder:** private `Xleia/train-libre-off-jp` (to be created)
- **Scope:** Japanese packaged food products, prioritizing review of FamilyMart, 7-Eleven, and Lawson coverage.

The two release tags are independent. The OFF channel must not alter, overwrite or delete the BLS release. Until an OFF build passes schema, nutrition-unit, licence, and update-safety validation, the Train Libre app should continue using the original OFF-JP release endpoint.

### Data licence and provenance

The OFF-derived database must attribute [Open Food Facts](https://world.openfoodfacts.org/) and comply with the [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/). Separate images and third-party retailer data require their own permission review. Do not publish unverified per-package nutrition figures as per-100g values.

### Release URLs

- BLS manifest: `https://github.com/Xleia/bls4-zh-catalog/releases/download/bls-foods-stable/catalog_manifest.json`
- Future OFF-JP manifest: `https://github.com/Xleia/bls4-zh-catalog/releases/download/off-foods-jp-stable/off_catalog_manifest_jp.json` (not available before first verified release)
