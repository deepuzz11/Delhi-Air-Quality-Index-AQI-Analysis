# Delhi Air Quality Index (AQI) Analysis

## Project Overview

This project involves an in-depth analysis of the Air Quality Index (AQI) for Delhi, utilizing a dataset with hourly pollutant measurements. The analysis aims to uncover patterns in air quality, understand seasonal variations, and explore correlations between different pollutants. Insights from this analysis can inform targeted strategies for improving air quality and public health initiatives in Delhi.

## Dataset

The dataset used for this analysis is `delhiaqi.csv`, which contains hourly measurements of various pollutants. The columns in the dataset are:

- `date`: Timestamp of the measurement in the format `YYYY-MM-DD HH:MM:SS`.
- `co`: Carbon monoxide levels (µg/m³).
- `no`: Nitric oxide levels (µg/m³).
- `no2`: Nitrogen dioxide levels (µg/m³).
- `o3`: Ozone levels (µg/m³).
- `so2`: Sulfur dioxide levels (µg/m³).
- `pm2_5`: PM2.5 levels (µg/m³, particulate matter ≤ 2.5 µm).
- `pm10`: PM10 levels (µg/m³, particulate matter ≤ 10 µm).
- `nh3`: Ammonia levels (µg/m³).

## Analysis and Results

### Seasonal Variation in PM2.5 Levels

An interactive box plot was created to visualize the distribution of PM2.5 levels across different seasons. This analysis helps identify how PM2.5 levels vary with seasonal changes.

- **File:** `seasonal_variation_pm25.html`
- **Key Findings:**
  - **Winter**: Highest median PM2.5 levels, with increased variability.
  - **Spring**: Lower median PM2.5 levels compared to Winter.
  - **Summer**: PM2.5 levels decrease further, showing lower median and variability.
  - **Autumn**: Similar to Spring, with moderate PM2.5 levels.

### PM2.5 Levels Over Time

An interactive line plot illustrates the temporal trends in PM2.5 levels, showing how they fluctuate over time and identifying any significant trends or anomalies.

- **File:** `time_series_pm25.html`
- **Key Findings:**
  - **Trend Analysis**: Monthly averages indicate periods of elevated PM2.5 levels, particularly during Winter months.
  - **Anomalies**: Significant spikes in PM2.5 levels can be observed during specific events or periods.

### Correlation Matrix of Pollutants

An interactive heatmap displays the correlation between different pollutants, providing insights into how various pollutants relate to each other.

- **File:** `correlation_matrix_heatmap.html`
- **Key Findings:**
  - **High Correlation**: Strong correlation observed between PM2.5 and PM10 levels, indicating that both particulate matter sizes often increase together.
  - **Moderate Correlation**: Notable correlations between NO2 and O3, suggesting related sources or environmental conditions.

## Usage Instructions

1. **Dependencies**: Ensure that the following Python libraries are installed: `pandas`, `matplotlib`, `seaborn`, `plotly`, `folium`.
2. **Data Preparation**: Download and place the `delhiaqi.csv` file in the project directory.
3. **Generate Visualizations**: Run the provided Python scripts to produce the HTML files with interactive visualizations.
4. **View Results**: Open the HTML files in a web browser to explore the interactive plots and heatmaps.

## Files

- `delhiaqi.csv`: Contains hourly AQI data for Delhi.
- `seasonal_variation_pm25.html`: Interactive box plot showing seasonal variation in PM2.5 levels.
- `time_series_pm25.html`: Interactive line plot of PM2.5 levels over time.
- `correlation_matrix_heatmap.html`: Interactive heatmap displaying the correlation matrix of pollutants.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
