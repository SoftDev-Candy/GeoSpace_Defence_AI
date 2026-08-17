<div align="center">

# GeoSpace Defence AI

**SAR Image Intelligence for Defensive Situational Awareness**

An end-to-end data and machine-learning project for turning Synthetic Aperture Radar imagery into structured, analyst-ready information.

![Python](https://img.shields.io/badge/Python-Active-3776AB?logo=python\&logoColor=white)
![Data](https://img.shields.io/badge/Data%20Pipeline-In%20Progress-555)
![Machine Learning](https://img.shields.io/badge/ML-Baseline%20Next-555)
![Status](https://img.shields.io/badge/Status-Active%20Development-2f7d32)

</div>

---

## What this project is

**GeoSpace Defence AI** explores how SAR imagery can move through a complete analytical workflow — from raw files to validated data, exploratory analysis, machine-learning experiments, evaluation, and eventually an analyst-facing interface.

The goal is not to build *another notebook that trains a classifier*. The project is being developed as a small, reproducible data system where every stage can be inspected, questioned, and improved.

<table>
<tr>
<td width="25%"><b>Data Foundation</b><br><sub>Inspect, validate, resize and encode SAR imagery.</sub></td>
<td width="25%"><b>Analysis</b><br><sub>Understand classes, distributions, image statistics and outliers.</sub></td>
<td width="25%"><b>Machine Learning</b><br><sub>Build baselines, evaluate mistakes and compare experiments.</sub></td>
<td width="25%"><b>Analyst Layer</b><br><sub>Turn predictions and metrics into usable visual reporting.</sub></td>
</tr>
</table>

## Current pipeline

```text
Raw SAR Data
     ↓
Inspection & Validation
     ↓
Preprocessing → 128 × 128
     ↓
Processed Dataset (.npz)
     ↓
EDA + Train / Validation / Test
     ↓
Baseline Model
     ↓
Evaluation & Error Analysis
     ↓
Structured Results
     ↓
Analyst Interface
```

## Dataset

The current build uses the **MSTAR-10-Classes** dataset package. It contains separate train/test directories and 11 supplied class folders. Images are standardized to **128 × 128**, labels are encoded, and reusable arrays are exported to `mstar_processed_128.npz`.

The processed artifact keeps `X_train`, `y_train`, `X_test`, and `y_test` separate so later experiments do not need to repeat the raw preprocessing stage.

## Development board

| Complete                 | In Progress          | Next                |
| ------------------------ | -------------------- | ------------------- |
| Dataset acquisition      | Validation split     | Baseline classifier |
| Structure inspection     | Exploratory analysis | Model evaluation    |
| Image preprocessing      | Dataset statistics   | Error analysis      |
| Label encoding           |                      | Experiment storage  |
| Processed dataset export |                      | Analyst dashboard   |

## Why SAR?

Radar imagery is useful in conditions where optical imagery can be limited. That makes SAR an interesting foundation for infrastructure monitoring, disaster-response analysis, logistics resilience, terrain/object analysis, and defensive situational awareness.

## Direction

The project is moving toward reproducible experiment tracking, queryable metadata, class-level evaluation, confusion analysis, misclassification inspection, and a compact interface for comparing results.

> **Data → Analysis → Intelligence → Analyst Support**

### Scope

This is an educational and defensive analytics project. It is intended for analysis, resilience research, monitoring, and decision support — **not weapon targeting, strike planning, or autonomous engagement**.

---

**Built incrementally. Documented as it evolves.**
