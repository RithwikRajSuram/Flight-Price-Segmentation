# Flight Price Segmentation using Hierarchical Clustering

## Project Overview
This project applies hierarchical clustering to flight ticket price data to identify natural pricing groups. The analysis uses the `price` column to segment flights into low, medium, and high price clusters. A dendrogram is used to visualize how similar prices are grouped together, and the silhouette score is used to evaluate how well the clusters are separated.

## Dataset
The dataset contains flight price records. In this analysis, the main feature used for clustering is:

- `price` - Flight ticket price

Sample data:

| price | cluster |
|---:|---:|
| 59222 | 2 |
| 68212 | 2 |
| 81900 | 1 |
| 94905 | 1 |
| 98937 | 0 |
| 121630 | 0 |

## Tools and Libraries Used
- Python
- Pandas
- Matplotlib
- SciPy
- Scikit-learn

## Methodology

### 1. Data Loading
The dataset was loaded using Pandas.

```python
import pandas as pd

data = pd.read_csv("Data-Week61.csv")
