# Manifold Learning Visualization on Digits Dataset

## Overview

This project applies multiple manifold learning techniques to the handwritten digits dataset to visualize high-dimensional data in 2D space. It compares how different algorithms represent the structure of the same dataset.

## Dataset

Loaded using:

```python
from sklearn.datasets import load_digits
```

* Contains images of handwritten digits (0–9)
* Each sample has 64 features (8×8 pixel values)

## Methods Used

The following dimensionality reduction techniques are applied:

### 1. t-SNE (t-Distributed Stochastic Neighbor Embedding)

* Focuses on preserving local structure
* Effective for visualizing clusters

### 2. Isomap

* Preserves global geometric structure
* Maintains geodesic distances between points

### 3. Locally Linear Embedding (LLE)

* Preserves relationships between neighboring points
* Suitable for non-linear manifolds

### 4. MDS (Multidimensional Scaling)

* Preserves pairwise distances between data points
* Useful for understanding similarity structure

## Workflow

1. Load dataset
2. Extract features (X) and labels (y)
3. Apply each dimensionality reduction technique
4. Plot 2D representations using scatter plots

## Technologies

* Python
* Matplotlib
* Scikit-learn

## Usage

1. Install dependencies:

```bash
pip install matplotlib scikit-learn
```

2. Run each script to visualize results:

```bash
python your_file.py
```

## Output

Each method generates a 2D scatter plot:

* Points represent digit samples
* Colors correspond to digit labels (0–9)
* Different methods show different clustering patterns

## Note

* Results may vary slightly due to randomness (except where `random_state` is fixed)
* Use Python 3.10 or 3.11 for best compatibility

## Author

Srishti Mishra
