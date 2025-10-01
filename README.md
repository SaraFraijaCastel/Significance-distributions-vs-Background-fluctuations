#  Significance Distributions vs Background Fluctuations

**Elevator pitch:** Data-science pipeline to test whether Gamma-Ray Burst (GRB) data in the **TeV** range indicate real emission by comparing observations to **simulated background fluctuations** using classical tests, **KDE**, and **Fisher’s method**.

---

## Data
- **Background fluctuations:** ~7,600 samples  
- **Observational data:** GRB detections from an observatory  
- **GRB metadata:** Positional/location info for each GRB

---

##  Pipeline
1. **Background characterization**
   - Correct positional errors per GRB
   - Test normality: **skewness, kurtosis, Kolmogorov–Smirnov (K-S)**
2. **Non-parametric background modeling**
   - **Kernel Density Estimation (KDE)** via SciPy
3. **GRB vs background comparison**
   - Statistical significance via **Fisher’s method**

---

## Methods & Tools
- **Stats:** Skewness, Kurtosis, K-S, Fisher’s method  
- **Modeling:** Non-parametric **KDE**  
- **Stack:** **Python**, **SciPy**, **NumPy**, **Pandas**, **Matplotlib**

---
## Repository structure

```text
├── Files/                     # CSV files
└── plots/                     # Distribution Plots
└── 1.FindingMax_Bkg.ipynb             # Background fluctuation max analysis
└── 2.FindingMax_Dat.ipynb             # Observed GRB data max analysis
└── 3.PlottingDistributions_and_FisherTest.ipynb  # Distribution plots + Fisher’s method
