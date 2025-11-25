# Project Outcome Analysis

Where are resources overallocated?

**Stakeholder:** Resource Manager

## Key Insights

- Bench time under 4 hours/week signals overallocation risk.
- Billable hours above 42/week precedes overallocation flags.
- FTE above 1.2 on a single initiative raises overload probability.

## Dataset

Primary file: `data/resource_utilization.csv`  
Target variable: `overallocated`

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook notebooks/analysis.ipynb
```


## Next Steps

**Done.** Weekly stakeholder report automation is implemented — see ### Implemented below.

---
*Analytics portfolio project — 2025-08*

<!-- build 5 -->

### Implemented

```bash
pip install -r requirements.txt
python scripts/weekly_report.py
```