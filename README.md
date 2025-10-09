# Early Onset Colon Cancer Trends
Tracking early-onset colon cancer trends across the globe with CI5plus data

---

## 📌 Project Overview
This project explores **early-onset colon cancer incidence trends** using data from **CI5plus** (Cancer Incidence in Five Continents).  Recent studies have raised concern about increasing rates of **early-onset colon cancer** (diagnoses before age 50).  This project investigates whether these trends represent a **true epidemiological shift** or mirror broader changes across all age groups.It forms part of a wider research effort into global cancer trends and contextual risk factors.

The notebook(s) in this repository focus on:
- Extracting and preparing CI5plus colon cancer incidence data
- Analyzing age-specific and early-onset (under 50 years) trends
- Comparing across countries/registries
- Building a foundation for subsequent analyses (breast, lung, prostate cancers)

---

## 🗂 Repo Structure
```
eo-colon-cancer-trends-ci5plus/
├── data/
│   ├── ci5_plus.csv
│   ├── cancer_dict.csv
│   └── registry_dict.csv
├── notebooks/
│   ├── 00_data-prep.ipynb
│   ├── 01_eda.ipynb
│   ├── 02_trend-analysis.ipynb
│   ├── 03_poisson-regression.ipynb
│   └── 04_stan-models.ipynb
├── scripts/
│   └── utils.py
├── docs/
│   └── poisson_model_interpretation.md
├── tests/
│   ├── README.md
│   └── test_poisson_model.py
├── results/
│   └── plots/
└── README.md
```

---

## 📊 Data Sources

CI5plus (Cancer Incidence in Five Continents, IARC)
🔗 https://ci5.iarc.fr/CI5plus/

(Note: Raw CI5plus data is not included in this repo. Please download directly from IARC or use synthetic data placeholders.)

---

## 📚 Documentation

- **[Poisson Model Interpretation Guide](docs/poisson_model_interpretation.md)**: Comprehensive guide to interpreting the Poisson regression model coefficients with explicit intercept

---

## 🧪 Testing

Run validation tests to verify model implementations:

```bash
python tests/test_poisson_model.py
```

See [tests/README.md](tests/README.md) for more details.

---

## 📜 License

This project is licensed under the **MIT License** – feel free to use and adapt with attribution.

---

## ✨ Next Steps

- Expand analysis to include other cancers (breast, lung, prostate).
- Integrate contextual country-level data (HDI, screening availability).
- Prepare manuscript-style outputs for academic submission.
