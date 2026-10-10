# Which Clock Drives Aircraft Failure Reporting?  
## Tail-Number Exposure Reconstruction From Public Records and Its Effect on Fleet Risk Rankings

This repository contains the Python code and derived tail-number-level exposure panel used in the manuscript:

> Yurtsever, Ö. (2026). *Which Clock Drives Aircraft Failure Reporting? Tail-Number Exposure Reconstruction From Public Records and Its Effect on Fleet Risk Rankings.* IEEE Transactions on Reliability.

---

## Overview

The study reconstructs flight cycles (FC) and flight hours (FH) for United States air-carrier aircraft from Bureau of Transportation Statistics (BTS) On-Time Performance records (2018–2024). The reconstructed exposure is linked to the FAA aircraft registry and to FAA Service Difficulty Reports (SDRs), validated against the SDR total-time and total-cycle fields, and used to test how fleet risk rankings depend on the chosen exposure clock (calendar, cycle, or hour).

The repository provides:
- reproducible code for data download, cleaning, record linkage, aggregation, modelling, and figure/table generation;
- a derived tail-number × quarter exposure panel;
- analysis-ready SDR aggregates;
- scripts to reproduce all tables and figures in the manuscript.

---

## Repository Contents

```text
.
├── code/               # Python scripts for preprocessing, linkage, modelling, and figures
├── data/               # Derived exposure panel and analysis-ready aggregates
│   ├── raw/            # (Not included) Raw BTS/FAA files should be downloaded from source
│   └── processed/      # Derived tail-number × quarter panel and linked SDR data
├── outputs/            # Generated figures and tables
├── requirements.txt    # Python dependencies
├── LICENSE             # License information
└── README.md
