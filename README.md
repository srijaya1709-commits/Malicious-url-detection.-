# Attack-Resistant Multi-Class Malicious URL Detection

Machine learning project that classifies URLs as benign, defacement,
phishing or malware, and aims to test how well the model resists
attacker-modified URLs.

**Dataset:** 651,191 URLs, 64 features
**Tools:** Python, pandas, NumPy, Matplotlib, Seaborn, SciPy
**Status:** Data cleaning and exploratory analysis complete; modeling in progress

## Key Insights
- The data is heavily imbalanced: malware is under 2% of URLs after cleaning.
- URL length and digit count differ significantly across URL types.
- HTTPS is not a safety signal: about 56% of malware URLs use it.
- Suspicious file extensions are most common in defacement URLs (~74%).
- `abnormal_url` and `//` are almost perfectly correlated (-0.99), so they are redundant.
