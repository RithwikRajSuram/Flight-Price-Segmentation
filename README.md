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

## Key Visualization
Dendrogram

The dendrogram shows how flight prices are merged into groups based on similarity. Prices that are closer together are joined earlier, while prices that are farther apart merge at higher levels in the graph.

## Conclusion

This project demonstrates how hierarchical clustering can be used to segment flight ticket prices without predefined labels. By using only the price feature, the model identified three natural pricing groups: low, medium, and high. The silhouette score of 0.6038 suggests that the clustering structure is meaningful and moderately well separated.
