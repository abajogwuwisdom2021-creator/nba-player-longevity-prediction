# NBA Player Longevity Prediction - Feature  Engineering
## project Overview
This repository implements a robust feature engineering pipeline in python using  'pandas', 'numpy', and 'seaborn'. The objective is to transform  raw historical NBA rookie box  score statistics into  a highly optimized,  clean dataset tailored for machine learning  models predicting whether aplayer's career will last 5+ years ('target_5yrs').
## Workflow Step Executed
1. **Target Variable Definition:** Explicitly mapped and validated the binary 'target_5yrs' column.
2. **Noise and Leakage Pruning:** Dropped categorical identity columns ('name') and structural artifact columns ('Unnamed: 0,').
3. **Data Integrity Check:** Verfied and confirmed that performance metrics contained no null values before modelling.
4. **Feature Synthesis:** Engineered two composite metrics:
- 'pts_per_min':Scoring density per unit of playtime.
- 'box_efficiency': A box score metrics combination score measuring raw court impact.
5. **Multicollinearity Elimination:** Computed feature correlations and removed redundant variations exceeding an absolute threshold of $0.90$.
##Workspace Artifacts Generated
- 'nba_feature_engineering.ipynb': Step-by-step executed jupyter Notebook pipeline.
- 'correlation_heatmap.png': Exported visual correlation matrix heatmap.
- 'clean_nba_longevity_feature.csv': Final model-ready dataset($1340\times15$).
