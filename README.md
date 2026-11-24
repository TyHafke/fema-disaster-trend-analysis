# U.S. Disaster Declaration Trends

## Overview

An exploratory data analysis and visualization project examining historical FEMA disaster declarations across the United States and its territories from 1953 to 2025.

This project investigates long-term trends in federal disaster declarations, changes in incident categories, and differences between historical time periods using Python.

## Research Objectives

- Examine changes in annual disaster declarations.
- Identify the most frequently declared disaster types.
- Compare disaster declaration trends across historical periods.
- Communicate findings through accessible data visualizations.

## Technologies Used

- Python
- pandas
- Matplotlib
- Jupyter Notebook
- Exploratory Data Analysis (EDA)

## Dataset

**Source:** Federal Emergency Management Agency (FEMA)

**Dataset:** Disaster Declarations Summaries v2

| Dataset Characteristic | Value |
|---|---:|
| Original Records | 69,936 |
| Variables | 28 |
| Unique Declarations Analyzed | 5,126 |
| Years Analyzed | 73 |
| Analysis Period | 1953–2025 |

[Original FEMA Dataset](https://www.fema.gov/openfema-data-page/disaster-declarations-summaries-v2)

[Dataset Documentation](data/README.md)

## Methodology

1. Import and inspect the original FEMA dataset.
2. Validate required variables and declaration identifiers.
3. Consolidate repeated records into unique disaster declarations.
4. Exclude incomplete fiscal year 2026.
5. Identify the seven most frequent incident categories.
6. Aggregate declarations by fiscal year and incident type.
7. Develop a streamgraph and annual trend visualization.
8. Compare declaration frequencies across historical periods.

## Visualization

![FEMA Disaster Declaration Trends](streamgraph.png)

The streamgraph illustrates changes in the frequency and composition of disaster declarations over time. The accompanying line chart displays annual declaration counts and a five-year rolling average.

## Key Findings

### Historical Trends

| Period | Average Annual Declarations |
|---|---:|
| 1980–1989 | 28.6 |
| 2015–2024 | 134.3 |

The more recent period averaged approximately 4.7 times as many annual disaster declarations.

### Most Frequent Incident Types

| Incident Type | Declarations |
|---|---:|
| Fire | 1,718 |
| Severe Storm | 1,124 |
| Flood | 912 |
| Hurricane | 453 |
| Tornado | 182 |
| Snowstorm | 171 |
| Biological | 167 |

### Additional Findings

- Fire and severe storm declarations accounted for the largest absolute increases between the two comparison periods.
- Fiscal year 2020 recorded the highest annual declaration count, with 315 declarations.
- Biological declarations contributed substantially to the increase observed in 2020.
- Hurricane declarations experienced a notable spike in 2005.

## Limitations

- Federal disaster declarations do not necessarily represent distinct physical disaster events.
- Changes in federal policies and reporting practices may influence historical trends.
- National-level analysis does not capture regional differences in disaster risk.
- Historical comparisons are descriptive and do not establish causation.
- Increasing declaration counts do not independently demonstrate increasing natural disaster frequency.

## Reproducing the Analysis

Install the required Python dependencies:

```bash
pip install -r requirements.txt
```

Open the Jupyter notebook:

```bash
jupyter notebook disaster_analysis.ipynb
```

Run all notebook cells to reproduce the analysis and visualization. The original dataset should be located in the `data` directory.

## Repository Contents

| File | Description |
|---|---|
| [Analysis Notebook](disaster_analysis.ipynb) | Python source code and analytical outputs |
| [Project Report](disaster-analysis-report.pdf) | Detailed methodology, findings, and conclusions |
| [Visualization](streamgraph.png) | Disaster declaration streamgraph and annual trends |
| [Data](data/) | Original dataset and documentation |
| [Requirements](requirements.txt) | Python dependencies |

## Future Improvements

- Explore state-level disaster declaration trends.
- Develop interactive geographic visualizations.
- Investigate regional differences in incident categories.
- Examine relationships between declaration trends and historical policy changes.

## Project Background

Originally developed as a CIS 320 final project at Grand Valley State University in June 2026. Subsequently refined to improve data validation, visualization quality, analytical accuracy, and reproducibility.

**Author:** Ty Hafke
