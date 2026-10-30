# Automobile Sales Analysis During Economic Recessions

## Project Overview

This project explores how economic recessions and other market factors relate to automobile sales. Using Python and a publicly hosted automobile sales dataset, the analysis compares recession and non-recession periods and presents trends through line charts, bar charts, scatter plots, bubble charts, and pie charts.

The work is contained in the Jupyter Notebook [`Final_Assignment1.ipynb`](Final_Assignment1.ipynb).

## Objectives

- Examine changes in average automobile sales over time, including recession periods.
- Compare automobile sales across recession and non-recession periods and vehicle types.
- Explore relationships between sales and GDP, consumer confidence, vehicle prices, unemployment, and seasonality.
- Analyze advertising expenditure by economic period and vehicle type.
- Communicate observations through clear data visualizations.

## Dataset

The notebook downloads `automobile-sales.csv` directly from the course-hosted source:

[Automobile Sales Dataset (CSV)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/d51iMGfp_t0QpO30Lym-dw/automobile-sales.csv)

Fields used in the analysis include `Year`, `Month`, `Recession`, `Automobile_Sales`, `Vehicle_Type`, `Advertising_Expenditure`, `GDP`, `Seasonality_Weight`, `Consumer_Confidence`, `Price`, and `unemployment_rate`.

The `Recession` field distinguishes recession (`1`) from non-recession (`0`) observations.

## Tools and Libraries

- **Python 3** — analysis and scripting
- **Jupyter Notebook** — interactive analysis
- **Pandas** — data loading, filtering, and aggregation
- **NumPy** — numerical computing
- **Matplotlib** — chart creation and customization
- **Seaborn** — statistical visualizations
- **Requests** — downloading the CSV dataset
- **Folium** — imported in the notebook, but not used in the displayed analysis

## Visualizations

The notebook includes:

1. **Yearly sales trends:** Average automobile sales by year, with recession annotations.
2. **Sales and advertising trends:** Average sales and advertising expenditure during non-recession periods.
3. **Recession comparisons:** Average sales during recession versus non-recession periods.
4. **Vehicle-type comparisons:** Average sales by vehicle category and economic period.
5. **GDP comparisons:** GDP trends during recession and non-recession periods.
6. **Seasonality:** A bubble-style scatter plot of monthly sales and seasonality weights.
7. **Consumer confidence and pricing:** Scatter plots against automobile sales during recessions.
8. **Advertising allocation:** Pie charts comparing expenditure by economic period and by vehicle type during recessions.
9. **Unemployment:** Automobile sales and unemployment rate by vehicle type during recessions.

## Key Observations

The notebook's commentary identifies the following patterns:

- Automobile sales are substantially lower during recessions, with executive and sports cars particularly affected.
- During non-recession periods, advertising expenditure and automobile sales generally move together. This is an **association, not evidence of causation**.
- Total advertising expenditure is higher in non-recession periods in the dataset.
- During recessions, higher unemployment is associated with lower automobile sales; several family-car categories show pronounced variation.

These are exploratory observations rather than causal conclusions or forecasts.

## Getting Started

### Prerequisites

Install Python 3 and Jupyter Notebook or JupyterLab.

### Installation

Clone the repository and enter its directory:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

Install the dependencies:

```bash
python -m pip install notebook pandas numpy matplotlib seaborn folium requests
```

### Run the Analysis

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `Final_Assignment1.ipynb` and select **Run All** to download the dataset and generate the visualizations. An internet connection is required to retrieve the CSV.

The notebook also contains `%pip install` cells for some libraries; the installation command above includes the additional packages imported by the notebook.

## Repository Structure

```text
.
├── Final_Assignment1.ipynb   # Data analysis and visualizations
└── README.md                 # Project documentation
```

## Skills Demonstrated

- Loading CSV data from a remote source
- Exploratory data analysis (EDA)
- Filtering and grouping data with Pandas
- Comparing economic periods and product segments
- Building and interpreting statistical charts
- Translating visual patterns into business observations

## Limitations

This is an exploratory visualization project. The charts show patterns and relationships in the supplied dataset but do not establish causality. No predictive model or formal statistical significance test is included in the notebook.

## Acknowledgments

The dataset is hosted on IBM Skills Network course infrastructure. This notebook was prepared as a data visualization assignment.
