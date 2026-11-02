---
name: geoskill-precision-farming-zoning
description: '多源数据标准化后用 K-means 聚类生成管理分区并给出每区建议。Standardizes multi-source layers, clusters them with K-means into management zones with per-zone advice.'
---

# 精准农业管理分区 | Precision Farming Management Zoning

(Fill in 2-3 paragraphs of Chinese introduction here: functionality, application scenarios, core algorithm.)

## Dependencies / 依赖

```bash
pip install 'numpy' 'rasterio' 'scikit-learn'
```

## Usage / 使用方法

### Basic usage

```bash
python geoskill-precision-farming-zoning.py --bbox 116.0 39.0 117.0 40.0 [other options]
```

### Example 1 (synthetic data, offline)

```bash
python geoskill-precision-farming-zoning.py --bbox 116.0 39.0 117.0 40.0 --synthetic --output-dir ./out
```

### Examples 2-5

(Add at least 4 real-world usage examples.)

## Output / 输出

| File | Format | Description |
|---|---|---|
| `result.tif` | GeoTIFF | Main output |
| `output-manifest.json` | JSON | Run manifest |

## Data Source / 数据源 / Source

(Describe the data source: free satellite data / local input / synthetic.)

## Privacy / 隐私声明 / Privacy

- Runs offline by default; `--synthetic` mode requires no network at all.
- All processing is performed locally; user data is never uploaded.

## License / License

MIT

---

> 中文完整版：需要时再读 [references/SKILL.zh-CN.md](references/SKILL.zh-CN.md)，不要默认全量加载。
