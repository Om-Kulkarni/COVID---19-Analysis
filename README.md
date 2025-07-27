## Example Forecast Visualization

Below is an example of a COVID-19 case forecast for India for April 2020, generated using Facebook Prophet. The dark blue line represents the predicted case count, while the light blue shaded area shows the 95% uncertainty interval.

![COVID-19 India Forecast April 2020](images/covid_india_april2020_forecast.png)

# COVID---19-Analysis

This project provides a comprehensive analysis and prediction of COVID-19 cases using various datasets and advanced forecasting techniques. The main analysis is performed in the Jupyter Notebook `COVID -19 Prediction(V2).ipynb`.

## Overview

The notebook covers:
- **Data Collection:** Reads multiple COVID-19 datasets, including global and India-specific data, from both local files and online sources.
- **Data Cleaning & Preparation:** Processes and merges datasets, handles missing values, and prepares data for analysis.
- **Forecasting:** Uses Facebook Prophet to forecast COVID-19 cases globally and for India, including predictions for confirmed and recovered cases.
- **Visualization:** Utilizes Plotly and Matplotlib for interactive and static visualizations, including:
  - Time series forecasts with uncertainty intervals
  - Animated global spread maps
  - Bar charts for top affected countries
  - Scatter plots relating cases to population, density, urbanization, and gender ratio
  - State-wise and age-group analyses
- **State-wise and Demographic Analysis:** Explores the impact of COVID-19 across Indian states, population density, urbanization, gender, and age groups.
- **Healthcare Infrastructure:** Analyzes hospital beds and testing facilities across states.

## Datasets

The analysis uses the following datasets (located in the `Datasets/` folder):
- `covid_19_data.csv`, `covid_19_india.csv`, `India_statewise_data.csv`, `IndividualDetails.csv`, `AgeGroupDetails.csv`, `HospitalBedsIndia.csv`, `ICMRTestingLabs.csv`, `StatewiseTestingDetails.csv`, `population_india_census2011.csv`, and time series data from Johns Hopkins University (JHU) via direct URLs.

## Forecasting Model

The notebook uses [Facebook Prophet](https://facebook.github.io/prophet/) for time series forecasting. Prophet is robust to missing data, outliers, and trend shifts, and is well-suited for data with strong seasonal effects.

## Visualizations

All plots are generated using Plotly for interactivity. To view the interactive plots, download and run the notebook locally.

## Requirements

- Python 3.x
- Jupyter Notebook
- pandas, numpy, matplotlib, seaborn, plotly, fbprophet

Install dependencies using pip:

```bash
pip install pandas numpy matplotlib seaborn plotly fbprophet
```

## Usage

1. Clone the repository and download the datasets (if not already present).
2. Open `COVID -19 Prediction(V2).ipynb` in Jupyter Notebook.
3. Run the notebook cells sequentially to reproduce the analysis and visualizations.

## Notes

- Some datasets are loaded from online sources; ensure you have an active internet connection.
- The notebook is best viewed in Jupyter for full interactivity.

## License

See [LICENSE](LICENSE) for details.
