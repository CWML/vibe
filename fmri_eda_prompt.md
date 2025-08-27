# fMRI Dataset EDA Prompt & Learning Guide

## Dataset Overview for Instructors

### What is the fMRI Dataset?
The seaborn fMRI dataset contains functional magnetic resonance imaging (fMRI) data measuring brain activity over time. This neuroimaging data captures BOLD (Blood Oxygen Level Dependent) signals from different brain regions during experimental conditions.

**Dataset Structure:**
- **1064 rows** of time-series measurements
- **5 columns**: subject, timepoint, event, region, signal
- **Real neuroscience data** from cognitive experiments
- **Longitudinal design** with repeated measurements

### Column Definitions
- **`subject`**: Participant ID (categorical)
- **`timepoint`**: Time point in the experiment (0-17, representing ~18 seconds)
- **`event`**: Experimental condition (stim vs cue)
- **`region`**: Brain region measured (frontal, parietal)
- **`signal`**: BOLD signal intensity (continuous, normalized)

### Why This Dataset is Perfect for Medical Audiences
1. **Clinical Relevance**: fMRI is widely used in neuroscience research
2. **Experimental Design**: Shows proper longitudinal data structure
3. **Real-World Application**: Demonstrates how brain activation is measured
4. **Research Methods**: Illustrates stimulus-response experimental paradigms

---

## EDA Prompt for VSCode + GitHub Copilot

**Copy and paste this prompt into VSCode with GitHub Copilot enabled:**

```
# fMRI Dataset Exploratory Data Analysis

I want to perform a comprehensive EDA on the seaborn fMRI dataset. This is neuroscience data measuring brain activity (BOLD signals) across different subjects, time points, experimental conditions, and brain regions.

Please help me:

## 1. Data Loading and Initial Exploration
- Load the fMRI dataset from seaborn
- Display basic info: shape, columns, data types, missing values
- Show first few rows and summary statistics
- Create a data dictionary explaining each variable

## 2. Distribution Analysis
- Plot the distribution of BOLD signal values
- Create histograms by brain region (frontal vs parietal)
- Show boxplots comparing signal distributions across experimental conditions (stim vs cue)
- Examine the distribution of timepoints and subjects

## 3. Time-Series Visualization
- Create line plots showing signal changes over timepoints
- Separate plots for each experimental condition (stim vs cue)
- Compare time-series between brain regions (frontal vs parietal)
- Add confidence intervals or error bars for multiple subjects

## 4. Group Comparisons
- Compare mean signal strength between brain regions
- Analyze differences between experimental conditions (stim vs cue)
- Create violin plots showing signal distributions by region and condition
- Statistical comparison of signal strength across groups

## 5. Subject-Level Analysis
- Show individual subject variability in responses
- Create a heatmap of subject responses across conditions
- Plot correlation matrix of variables
- Identify potential outlier subjects or time points

## 6. Advanced Visualizations
- Create a comprehensive dashboard-style figure with subplots
- Use seaborn's FacetGrid for multi-panel comparisons
- Generate interaction plots (region × condition × time)
- Create publication-ready figures with proper labels and styling

## 7. Statistical Insights
- Calculate correlation coefficients between variables
- Perform basic statistical tests (t-tests, ANOVA if appropriate)
- Identify peak activation timepoints for each condition
- Summarize key findings from the EDA

Please use seaborn and matplotlib for visualizations, pandas for data manipulation, and include clear comments explaining each step. Make the code educational and easy to follow for learners.

Also suggest what machine learning analyses could follow this EDA (classification, regression, time-series analysis, clustering, etc.)
```
