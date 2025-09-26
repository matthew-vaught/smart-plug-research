# Smart Plug Energy Consumption Research 🔌

This repository contains notebooks and supporting files for my research on **smart plug energy consumption** patterns across buildings on a college campus.

---

## Background & Motivation

This project investigates how energy usage varies across buildings and devices when measured at the plug level. The motivation was to:

- Understand how much power is consumed by devices connected through smart plugs.  
- Compare plug-level usage with total building loads to identify discrepancies.    
- Visualize consumption patterns across time (daily, weekly, seasonal) and geography.  

The ultimate goal is to highlight opportunities for more efficient energy use on campus.

---

## Data & Sources

- **Smart plug data**: ~1 million rows of timestamped plug-level power readings.  
- **Columns include**: timestamp, plug ID, power consumption (kW).  
- **Granularity**: data recorded at 1-minute and 15-minute intervals.  
- **Building-level data**: aggregated total load from building meters for correlation studies.  

---

## Methods & Tools

- **Data Cleaning & Aggregation**:  
  - Converted minute-level readings into hourly, daily, and weekly consumption trends.  
  - Filtered erroneous values and standardized timestamps.  

- **Visualization & Analysis**:  
  - Heatmaps, line charts, and animated plots to show seasonal and weekly patterns.  
  - Geospatial heatmaps across California buildings using H3 hex bins.  

- **Statistical Methods**:  
  - Pearson correlation between plug-level and building-level usage.
  - Peak load identification to study high-demand hours.

- **Tools**: Python — Pandas, NumPy, Matplotlib, Plotly, H3, scikit-learn.

---

## Key Findings & Insights

- Plug-level consumption patterns clearly reflected **daily, weekly, and seasonal cycles**.  
- Strong correlations (but not perfect) between plug-level sums and building meter totals revealed how much of each building’s consumption could be explained by monitored plugs.    
- Geospatial heatmaps provided a new perspective on how energy consumption changes across campus geography.  

---

## Repository Structure

```
smart-plug-research/
│
├── Correlational Analysis Notebooks/ # notebooks analyzing correlation between plug and building data
├── Data Cleaning Notebook/ # preprocessing and cleaning scripts
├── Data Visualization Files/ # saved visual outputs (plots, animations, heatmaps)
├── Data Visualization Notebooks/ # notebooks for time series and geospatial visualizations
└── README.md
```

---

## How to Explore / Use This Repo

1. Start with **Data Cleaning Notebook/** to understand how raw plug data was preprocessed.  
2. Explore **Correlational Analysis Notebooks/** to see comparisons between building load and smart plug data.  
3. Review **Data Visualization Notebooks/** for heatmaps, animations, and geospatial analysis.  
4. Check **Data Visualization Files/** for saved plots and figures used in presentations.
