# 🚗 US Auto Insurance Benchmark Dataset (2026 Actuarial Index)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Dataset: 2026 US Rates](https://img.shields.io/badge/Dataset-2026_US_Auto_Insurance-emerald.svg)](https://autoinsure.online)
[![Vehicles: 196 US Models](https://img.shields.io/badge/Vehicles-196_US_Models-blue.svg)](https://autoinsure.online/vehicles)
[![States: 50 US States](https://img.shields.io/badge/States-50_US_States-indigo.svg)](https://autoinsure.online/states)
[![Coverage: 98.4% Fleet](https://img.shields.io/badge/Coverage-98.4%25_US_Fleet-success.svg)](https://autoinsure.online)
[![Maintained by](https://img.shields.io/badge/Maintained_by-AutoInsure.online-blue.svg)](https://autoinsure.online)

An open-access, actuarially audited reference dataset containing **2026 statutory minimum insurance mandates across all 50 US states**, **underwriting rate benchmarks for all 196 passenger vehicle models in America (covering 98.4% of all registered passenger vehicles)**, and **7,500+ localized state-by-vehicle rate calculations**.

Maintained by the editorial and actuarial research team at [AutoInsure.online](https://autoinsure.online).

---

## 📌 Primary Research Hubs & Calculators

- 🌐 **Official Portal & Interactive Estimator:** [https://autoinsure.online](https://autoinsure.online)
- 📊 **2026 Lowest Cost Vehicles Ranking (196 Models):** [https://autoinsure.online/cheapest-cars-to-insure](https://autoinsure.online/cheapest-cars-to-insure)
- 🚘 **Vehicle Insurance Profiles & Risk Tiers (All 196 Models):** [https://autoinsure.online/vehicles](https://autoinsure.online/vehicles)
- ⚖️ **50-State Statutory Mandate Directory:** [https://autoinsure.online/states](https://autoinsure.online/states)
- 🧮 **Claim vs. Out-of-Pocket Calculator:** [https://autoinsure.online/claim-calculator](https://autoinsure.online/claim-calculator)
- 🏎️ **Vehicle vs. Vehicle Head-to-Head Comparator:** [https://autoinsure.online/compare-vehicles](https://autoinsure.online/compare-vehicles)
- 📰 **Actuarial Blog & Research Guides:** [https://autoinsure.online/blog](https://autoinsure.online/blog)

---

## 📁 Repository Structure

```
├── data/
│   ├── us_state_insurance_benchmarks_2026.csv   # Statutory limits & full coverage rates for 50 states
│   ├── us_vehicle_insurance_rates_2026.csv      # Underwriting benchmarks for 196 US vehicle models
│   └── autoinsure_index_2026.json               # Full unified JSON dataset (196 vehicles + 50 states)
├── CITATION.cff                                 # Academic citation metadata
├── LICENSE                                      # Creative Commons Attribution 4.0 International
└── README.md                                    # Documentation, catalog index & methodology
```

---

## 🔍 Key National Benchmarks (2026 Composite)

| Metric | 2026 National Benchmark | Reference Source |
| :--- | :--- | :--- |
| **National Average Full Coverage** | **$2,388 / year** ($199 / month) | [AutoInsure National Index](https://autoinsure.online) |
| **National Average Minimum Liability** | **$784 / year** ($65 / month) | [AutoInsure State Hub](https://autoinsure.online/states) |
| **#1 Lowest Cost Vehicle to Insure** | **Honda Odyssey** ($1,480 / yr) | [Cheapest Cars Guide](https://autoinsure.online/cheapest-cars-to-insure) |
| **#2 Lowest Cost Vehicle to Insure** | **Toyota Sienna** ($1,490 / yr) | [Toyota Sienna Guide](https://autoinsure.online/vehicle/toyota-sienna) |
| **#3 Lowest Cost Vehicle to Insure** | **Subaru Forester** ($1,510 / yr) | [Subaru Forester Guide](https://autoinsure.online/vehicle/subaru-forester) |
| **Highest Average State (Full Coverage)** | **Michigan** ($3,450 / yr) | [Michigan Insurance Guide](https://autoinsure.online/state/michigan) |
| **Lowest Average State (Full Coverage)** | **Maine** ($1,280 / yr) | [Maine Insurance Guide](https://autoinsure.online/state/maine) |

---

## 🏎️ Vehicle Catalog Breakdown (196 Models)

The dataset covers **196 production passenger vehicles** sold in the United States, categorized by segment:

| Segment | Model Count | Benchmark Premium Range | Dominant Risk Factor |
| :--- | :---: | :--- | :--- |
| **SUVs & Crossovers** | 78 Models | $1,510 – $2,380 / yr | High safety score offsets curb weight; low collision loss |
| **Sedans & Hatchbacks** | 46 Models | $1,590 – $2,490 / yr | Commuter exposure, moderate catalytic theft risk |
| **Pickup Trucks** | 22 Models | $1,720 – $2,410 / yr | High vehicle mass protects occupants; higher third-party property damage |
| **Electric Vehicles (EVs)** | 28 Models | $1,940 – $3,250 / yr | Proprietary structural gigacastings, battery pack replacement costs |
| **Minivans** | 6 Models | $1,480 – $1,620 / yr | **Lowest casualty risk** in US fleet due to cautious family demographics |
| **Luxury & Performance** | 16 Models | $2,200 – $3,450 / yr | Elevated horsepower, certified technician hourly labor rates |

---

## 📐 Actuarial Methodology & Rules

This dataset integrates state insurance department regulatory filings, NHTSA 5-star crash safety ratings, and ISO/NAIC loss-cost ratios.

### The Actuarial 10% Replacement Rule
When vehicle collision and comprehensive premiums exceed **10% of the vehicle's actual cash value (ACV) minus the deductible**, maintaining full physical damage coverage becomes actuarially disadvantageous. Full mathematical breakdown available at:  
👉 [The Actuarial 10% Rule: When to Drop Collision & Comprehensive](https://autoinsure.online/blog/actuarial-10-percent-rule-drop-full-coverage)

### Localized State-by-Vehicle Matrix Formula
State rates are computed from each state's regulatory cost multiplier $M_s$ applied to the baseline vehicle loss-cost $L_v$:
$$R_{v,s} = L_v \times M_s \times \Phi_{\text{statutory}}$$
Where $\Phi_{\text{statutory}}$ adjusts for compulsory PIP, uninsured motorist mandates, and pure comparative fault environments. Full localized matrices are indexed live at:  
👉 `https://autoinsure.online/rates/[vehicle-slug]-in-[state-slug]`

---

## 📖 Citation

If you use this dataset in financial research, journalism, educational coursework, or machine learning models, please cite:

### APA:
```text
Rostova, E., & Vance, M. (2026). 2026 United States Auto Insurance Actuarial Benchmark Index (196-Vehicle Dataset). AutoInsure.online. Retrieved from https://autoinsure.online
```

### BibTeX:
```bibtex
@misc{autoinsure2026index,
  author = {Elena Rostova, FCAS and Marcus Vance, CPCU},
  title = {2026 United States Auto Insurance Actuarial Benchmark Index (196-Vehicle Dataset)},
  year = {2026},
  publisher = {AutoInsure.online},
  howpublished = {\url{https://autoinsure.online}}
}
```

---

## ⚖️ License

This dataset is made available under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license. You are free to share and adapt the material for any purpose, provided appropriate credit is given to [AutoInsure.online](https://autoinsure.online).
