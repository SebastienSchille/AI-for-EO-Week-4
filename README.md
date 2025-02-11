# Project Context

This section covers unsupervised learning with a practical focus, avoiding deep theoretical discussions. The emphasis is on applying these methods in EO scenarios, particularly for classification tasks, where they excel at identifying patterns in unlabeled data.

Key topics:

* Detecting structure and relationships in datasets without predefined categories.
* Primary tasks:
  * Classifying sea ice and leads using Sentinel-2 optical data.
  *  Classifying sea ice and leads using Sentinel-3 altimetry data.

# Methods used

## K-means Clustering

K-means is an unsupervised learning algorithm used to partition data into k predefined clusters based on feature similarity. It works by iteratively assigning data points to the nearest centroid and updating centroids until minimal variation within clusters is achieved.

### Why K-means?

* Suitable for datasets with unknown structure (ideal for exploratory analysis).
* Simple and scalable for large datasets.

### Key Components:

* Choosing k: The number of clusters must be predefined.
* Centroid Initialization: Initial placement affects results.
* Assignment Step: Data points assigned to nearest centroid (using Euclidean distance).
* Update Step: Centroids recalculated based on assigned points.

## Gaussian Mixture Models (GMM)

GMM is a probabilistic model that represents data as a mixture of multiple Gaussian distributions, each with its own mean and variance. It is used for clustering and density estimation, offering a more flexible alternative to K-means.

### Why GMM for Clustering?

* Soft Clustering: Assigns probabilities to data points for each cluster rather than hard assignments.
* Flexible Cluster Shapes: Allows clusters to have different sizes and orientations, adapting to complex data distributions.

### Key Components:

* Number of Components: Similar to k in K-means, defines the number of Gaussian distributions.
* Expectation-Maximization (EM) Algorithm: Iteratively refines cluster assignments and model parameters.
* Covariance Type: Defines cluster shape (e.g., spherical, elliptical).

### The EM Algorithm:

* Expectation Step (E-step): Computes the probability of each point belonging to each cluster.
* Maximization Step (M-step): Updates Gaussian parameters (mean, covariance, mixing coefficient) to maximize data likelihood.
* Repeats until convergence.

# Getting Started

## Packages

## Files

# Roadmap

- [ ] Step 1
- [ ] Step 2

# Contact

Sebastien Schille - sebastien.j.schille@gmail.com

Project link - https://github.com/SebastienSchille/AI-for-EO-Week-4

# Acknowledgments

This code was created for the taught module GEOL0069 at UCL - ran by Dr. Michel Tsamados



