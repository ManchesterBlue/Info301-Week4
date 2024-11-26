# Infovis Redesign Project

## Introduction

This project focuses on redesigning visualizations from the paper **“Dead or Alive: Continuous Data Profiling for Interactive Data Science”**, which introduces **AutoProfiler**, a tool for automating data profiling in Jupyter notebooks. AutoProfiler enhances exploratory data analysis (EDA) by providing live, continuously updating visualizations and metrics, reducing manual effort and enabling real-time data verification.

The study compares two tools:
- **AutoProfiler**: Offers live updates and automated visualizations.
- **StaticProfiler**: Requires manual invocation and displays static visualizations.

The evaluation includes a user study analyzing performance across the following metrics:
1. Number of insights found (out of 16).
2. Number of unique dataframes explored.
3. Number of unique columns explored.
4. Number of selection exports.
5. Number of template exports.

---

## Visualizations

### Original Visualization
The original visualizations (Figure 6) are box plots comparing the performance of AutoProfiler and StaticProfiler across the five metrics. While these plots provide a clear comparison of central tendencies and variability, they lack sufficient contextual information and accessibility features.

### Redesigned Visualization
The redesigned visualizations (Figure 7) improve upon the original by:
1. Adding annotations to explain the significance of each metric.
2. Using color and hatching patterns for better accessibility.
3. Including sample size and statistical significance (e.g., p-values).
4. Rearranging metrics to highlight the most important ("Number of insights found").
5. Simplifying the display of mean values for clarity.

---

## Implementation

### Code Highlights
Two Python scripts were used to generate the visualizations:
1. **Basic Visualizations**:
   - Horizontal box plots with color coding (blue for AutoProfiler, orange for StaticProfiler).
   - Inclusion of mean values (µ) for each tool.
2. **Enhanced Visualizations**:
   - Contextual annotations for each metric.
   - Improved accessibility with hatching patterns.
   - Indicators for sample size and statistical significance.
   - Emphasis on key metrics using a hierarchical layout.

### Code Repository
The full code is available in the accompanying [Google Colab Notebook](https://colab.research.google.com/drive/1alLABYeaqmvYzaTXCQwO2xcE4itBjMmw?usp=sharing).

---

## Reflection on Visualization Design

### Strengths of the Redesigned Visualization
- **Clarity**: Annotations provide context for interpreting the metrics.
- **Accessibility**: Hatching patterns enhance readability for colorblind users.
- **Transparency**: Statistical significance and sample size improve the credibility of the results.

### Limitations
- The inclusion of annotations may lead to visual clutter in some cases.
- Statistical annotations are limited to selected metrics, which may confuse viewers.

---

## Insights from LLM Feedback

A Large Language Model (LLM) was used to critique and refine the visualizations. Key feedback included:
- Identifying issues with accessibility and clutter in the original design.
- Suggesting actionable improvements like adding annotations and hatching patterns.
- Highlighting the need for statistical context to support the observed differences.

While the LLM provided valuable insights, it occasionally lacked domain-specific knowledge to fully address the context of metrics such as "Number of template exports."

---

## Data and Resources

- **Paper**: [Dead or Alive: Continuous Data Profiling for Interactive Data Science](https://arxiv.org/pdf/2308.03964)
- **Colab Notebook**: [Visualization Code](https://colab.research.google.com/drive/1alLABYeaqmvYzaTXCQwO2xcE4itBjMmw?usp=sharing)
