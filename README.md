# PlaceSAVER: A Python Toolkit for CA1 Place Cell Analysis

**PlaceSAVER** (Hippocampal CA1 **Place**cell **S**imulation, **A**nalysis, **V**isualization, of **E**ncoding, and **R**emapping). This Python toolkit provides capabilities for generating synthetic calcium imaging datasets, performing place cell analyses, and creating visualizations.



## Overview

PlaceSAVER provides tools for computational place cell research by offering:

1. **Data Simulation**: Generate synthetic calcium imaging datasets that model hippocampal place cell behavior
2. **Analysis Pipeline**: Analyze both real and synthetic data using established computational methods
3. **Visualization Tools**: Create figures for data exploration and publication
4. **Ground Truth Validation**: Compare analytical results against known synthetic data properties



## Applications

### Educational Use
- **Student Training**: Generate synthetic datasets to teach place cell concepts with hands-on experience
- **Visual Learning**: Clear visualizations demonstrate spatial tuning, place fields, and population dynamics  
- **Progressive Complexity**: Move from basic single-cell metrics to advanced population analyses with known ground truth

### Hypothesis Generation
- **Cell Type Comparisons**: Test layer-specific hypotheses (Deep vs. Superficial CA1 cells) and projection-specific properties (EC-projecting vs. LS-projecting neurons)
- **Environmental Manipulations**: Simulate remapping experiments with controlled context changes, reward relocations, and time delays
- **Parameter Exploration**: Systematically vary experimental conditions to test specific predictions

### Method Validation
- **Algorithm Testing**: Validate new analytical approaches against datasets with known properties
- **Parameter Optimization**: Optimize spatial binning, smoothing, and significance thresholds using ground truth feedback
- **Robustness Assessment**: Test method performance across different noise levels and data complexities

### Research Applications
PlaceSAVER can be useful for studies investigating:
- **Place cell remapping** in response to environmental changes
- **Neural population activity** during spatial navigation
- **Position decoding** from neural activity patterns
- **Method testing** using synthetic datasets with known ground truth
- **Comparative analysis** across experimental conditions



## Toolkit Capabilities

### Data Simulation
Generate realistic synthetic calcium imaging datasets with:
- **Virtual reality environments** (linear tracks with configurable parameters)
- **Biologically accurate calcium dynamics** (GCaMP variant modeling with realistic noise)
- **Diverse cell populations** (user-defined subgroups: Deep/Superficial layers, EC-projecting/LS-projecting neurons)
- **Multiple experimental paradigms** (baseline, context changes, reward relocations, time delays)
- **Complete ground truth metadata** for method validation

### Single-Cell Analysis  
Extract place cell properties including:
- **Spatial tuning and place field detection** (automated identification with size/position metrics)
- **Information content measures** (Skaggs spatial information, sparsity/selectivity indices)
- **Activity characterization** (peak/mean rates, event amplitude/width/frequency)
- **Stability assessment** (session-half correlations, lap-by-lap drift analysis)
- **Statistical validation** (shuffle testing, significance assessment, confidence intervals)

### Population-Level Analysis
Analyze collective neural dynamics through:
- **Population vector correlations** (spatial correlation analysis across neural populations)
- **Decoding approaches** (Linear Regression, Naive Bayes with cross-validation frameworks)
- **Dimensionality reduction** (PCA, t-SNE, UMAP for neural manifold analysis including topology-aware methods)
- **Representational similarity analysis** (population-level similarity matrices)
- **Correlation networks** (pairwise correlation analysis within and between cell subtypes)

### Cross-Condition Analysis
Compare neural responses across experimental manipulations:
- **Remapping characterization** (place field property changes across conditions)
- **Stability quantification** (cross-trial consistency and correlation analysis)
- **Population comparisons** (group-level statistical analysis and visualization)
- **Comprehensive significance testing** (including shuffle analysis visualization)

### Visualization and Output
Create publication-ready figures with:
- **Multi-scale visualizations** (single-cell tuning curves, population heatmaps, manifold plots)
- **Cross-condition comparisons** (side-by-side grids, overlay plots, statistical summaries)
- **Multiple output formats** (PNG, EPS, SVG with configurable parameters)
- **Automated batch processing** and memory management for large datasets

### Getting Started
1. **Configure experiments** using YAML parameter files
2. **Generate synthetic data** with known ground truth properties  
3. **Run analysis pipeline** sequentially or in parallel
4. **Validate methods** by comparing results against ground truth
5. **Apply to real data** using the same analytical framework

**Technical Requirements**: Python 3.11+, scientific computing stack (pandas, numpy, scipy, sklearn, matplotlib, seaborn), optional advanced libraries (UMAP, statsmodels)



## Extending the Toolkit

The scripts are designed to be modifiable. Researchers can:
- Modify existing analysis methods in the scripts
- Add new visualization approaches
- Implement additional statistical tests
- Use the synthetic data generation for testing new methods

PlaceSAVER provides a foundation for place cell analysis, offering both data generation and analysis tools for computational neuroscience research. 
