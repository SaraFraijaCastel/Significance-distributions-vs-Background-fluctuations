Significance Distributions vs Background Fluctuations

This project explores whether data in the teraelectronvolt (TeV) energy range could represent genuine emission, by testing Gamma-Ray Burst (GRB) observations against simulated background fluctuations.

Data
	•	Background fluctuations: ~7,600 samples
	•	Observational data: Gamma-ray burst detections from an observatory
	•	GRB information: Includes positional and location data

Pipeline
	1.	Background Characterization
	•	Corrected positional errors for each GRB
	•	Tested normality (skewness, kurtosis, Kolmogorov–Smirnov test)
	2.	Non-Parametric Background Modeling
	•	Applied Kernel Density Estimation (KDE) with SciPy
	3.	GRB vs Background Comparison
	•	Measured statistical significance using Fisher’s method

Methods & Tools
	•	Statistical tests for normality
	•	Non-parametric density estimation (KDE)
	•	Significance testing to distinguish GRB signals from background fluctuations
	•	Python | SciPy | NumPy | Pandas | Matplotlib
