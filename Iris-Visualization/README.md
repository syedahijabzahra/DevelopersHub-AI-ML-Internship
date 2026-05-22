# Task 1: Exploring and Visualizing the Iris Dataset

## Objective
Load, inspect, and visualize the Iris dataset to understand feature distributions, relationships, and outliers.

## Dataset
- **Name:** Iris Dataset
- **Source:** Built into seaborn (`sns.load_dataset("iris")`) — no download needed
- **Size:** 150 rows × 5 columns
- **Classes:** Setosa, Versicolor, Virginica (50 samples each)

## Libraries Used
`pandas` `numpy` `matplotlib` `seaborn`

## Models Applied
No model — this task focuses on EDA and visualization only.

## Steps
1. Load and preview the dataset
2. Inspect shape, types, missing values, and statistics
3. Scatter plots — feature relationships by species
4. Histograms — value distributions per feature
5. Box plots — spread and outliers per species
6. Pair plot — all feature combinations
7. Correlation heatmap

## Key Results & Findings
- Dataset is clean — no missing values, perfectly balanced classes
- Petal features (length & width) separate species far better than sepal features
- Iris Setosa is clearly distinct from the other two species
- Versicolor and Virginica overlap slightly
- Petal length and petal width are highly correlated (r = 0.96)
- Sepal width has weak correlation with all other features
