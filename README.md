

# Brazilian Chamber Voting Networks

Network-based analysis of roll-call voting patterns in the Brazilian Chamber of Deputies using statistical similarity, graph modeling, and network visualization.

## Overview

This project analyzes roll-call voting behavior in the Brazilian Chamber of Deputies by transforming legislative voting records into statistical similarity matrices and weighted networks.

The analysis is performed at two levels:

- political parties;
- individual deputies.

Voting profiles are compared using correlation-based similarity measures. These similarities are then transformed into weighted graphs that can be analyzed using Network Science methods.

The project combines:

- data processing;
- exploratory data analysis;
- statistical similarity analysis;
- graph modeling;
- network metrics;
- network visualization;
- temporal comparison across legislative periods.

## Analytical Pipeline

```text
Raw Voting Records
        ↓
Data Cleaning
        ↓
Vote Encoding
        ↓
Voting Matrix
        ↓
Similarity Matrix
        ↓
Threshold Selection
        ↓
Network Construction
        ↓
Network Visualization
        ↓
Network Metrics
        ↓
Sensitivity Analysis

## Notebooks

| Notebook | Conteúdo |
|---|---|
| `01_Descriptive_Analysis.ipynb` | Análise descritiva dos dados de votação. |
| `02_Party_Voting_Networks.ipynb` | Redes de votação entre partidos. |
| `03_Deputy_Voting_Networks_Refactored_Optimized_FIXED.ipynb` | Redes de votação entre deputados. |
| `04_Deputy_Network_Descriptive_Results.ipynb` | Resultados descritivos das redes de deputados. |
| `Methodoly.ipynb` | Metodologia. |

## Como reproduzir

```bash
python -m venv .venv
source .venv/bin/activate   # no Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Execute os notebooks na ordem numérica. O layout ForceAtlas2 usa o pacote opcional `fa2`
(`pip install fa2`); sem ele, os notebooks seguem com os demais layouts.
