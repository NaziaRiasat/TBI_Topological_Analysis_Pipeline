# TBI Topological Analysis Pipeline

Proof-of-concept pipeline for topological feature extraction 
and statistical analysis of functional brain networks.

## Based on
- Centeno et al. (2022) — network and topological neuroscience tutorial
- Santos et al. (2019) — topological phase transitions in brain networks

## Pipeline
1. Generate synthetic connectivity matrices (healthy vs TBI)
2. Run filtration (ε sweep 0.02 → 0.65)
3. Compute Euler characteristic, Betti numbers, phase transitions
4. Extract 15 topological features per subject
5. Group comparison, classification, cognitive score correlation

## Key finding (synthetic data)
- 14/15 features significant (p < 0.05)
- Classification AUC = 1.0 (synthetic — expect ~0.75-0.85 on real data)
- Euler entropy AUC correlates with IQ at r = 0.44

## Dependencies
numpy, networkx, scipy, sklearn, matplotlib
