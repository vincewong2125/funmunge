# Gene Co-Expression Network Analysis

## Overview

This Python notebook contains code for analyzing and visualizing co-expression networks of genes associated with specific body parts. The code uses the `genemunge` package to process gene expression data, calculate correlations, and create interactive network visualizations.

## Usage

1. **Setup GeneMunge Objects**: The script sets up objects to describe and normalize genes using the GeneMunge package.

2. **Retrieve Expression Data**: It retrieves expression data for the specified body part in healthy tissue (in TPM units) using the GeneMunge package.

3. **Generate Synthetic Samples**: Synthetic samples are generated from a Gaussian distribution to approximate gene expression levels.

4. **Normalize Synthetic Data**: The synthetic data is normalized to TPM (Transcripts Per Million) values using the GeneMunge package.

5. **Calculate Correlation Matrix**: The script calculates the correlation matrix of gene expression to identify co-expressed genes.

6. **Construct Adjacency Matrix**: An adjacency matrix is constructed based on a correlation threshold to identify significant co-expressed gene pairs.

7. **Create Network Graph**: A networkx graph is created from the adjacency matrix, and node degrees are calculated.

8. **Define Layout**: A layout for the network graph is defined using networkx.

9. **Generate Plotly Traces**: Plotly traces for edges and nodes are generated, with node degrees influencing colors and sizes.

10. **Build Plotly Figure**: A Plotly figure for visualization is built and returned by the script.

## Examples

The notebook provides examples of co-expression network analysis for three different body parts: lung, uterus, and muscle.

## Additional Functionality

The notebook includes a function, `get_connected_nodes_and_subset(node_id, node_data_sorted, adjacency_matrix)`, for retrieving connected nodes and subsets of the node data. This can be useful for more in-depth analysis of specific genes or nodes within the network.
