
# COVID-19 Global Data Tracker

This Jupyter Notebook, authored by Samira Hassannoor, analyzes global COVID-19 trends, including cases and deaths, using the [Johns Hopkins University (JHU) CSSE COVID-19 dataset](https://github.com/CSSEGISandData/COVID-19). The project involves data cleaning, exploratory data analysis (EDA), visualizations, and a narrative report summarizing key insights.

## Objectives
- Import and clean COVID-19 global data from JHU CSSE.
- Analyze time trends for cases and deaths.
- Compare metrics across countries (Kenya, United States, India).
- Visualize trends using charts and a choropleth map.
- Summarize findings in a clear, reproducible report.

## Prerequisites
- Dataset: The notebook uses JHU’s time-series data, fetched from:
  - [Confirmed cases](https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_global.csv)
  - [Deaths](https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_deaths_global.csv)
- No local dataset files are required, as the notebook loads data from URLs.
- Libraries: Ensure pandas, matplotlib, seaborn, and plotly are installed. Install them using:
  ```bash
  pip install pandas matplotlib seaborn plotly
  ```

## Steps
### Step 1: Data Loading & Exploration
- Load the JHU CSSE dataset using pandas and explore its structure.

### Step 2: Data Cleaning
- Clean the dataset by filtering relevant countries, reshaping the time-series format, and handling missing values.

### Step 3: Exploratory Data Analysis (EDA)
- Analyze trends in cases, deaths, and calculate death rates.

### Step 4: Choropleth Map
- Visualize total cases by country on a world map using Plotly.

### Step 5: Insights & Narrative
- Key insights, conclusions, and future work suggestions.

## Key Insights
1. Case Trends: The United States reported the highest total cases, exceeding 100 million by mid-2022, followed by India with over 40 million, while Kenya had significantly lower cases (under 1 million), likely due to population differences and testing capacity.
2. Death Rates: The death rate (total deaths / total cases) was highest in the United States, averaging around 1.2% by late 2022, compared to India’s 1.1% and Kenya’s 1.7%, reflecting variations in healthcare systems and reporting accuracy.
3. Anomalies: Spikes in cases were observed in India around April 2021, likely due to the Delta variant, with daily cases peaking at over 400,000.
4. Global Perspective: The choropleth map highlights high case density in North America, Europe, and parts of Asia, with lower reported cases in Africa, possibly due to limited testing infrastructure.
5. Data Limitations: The JHU dataset provides robust case and death data but lacks vaccination data, limiting analysis of immunization trends.

## Conclusion
This analysis reveals significant variations in COVID-19 impacts across countries, driven by factors like population, healthcare infrastructure, and testing capacity. The visualizations and metrics provide a clear picture of global trends, suitable for policymakers, public health researchers, or data enthusiasts.

## Future Work
- Integrate vaccination data from sources like Our World in Data to analyze immunization trends.
- Develop an interactive dashboard using Streamlit for user-driven exploration.
- Investigate the impact of specific policies (e.g., lockdowns, travel bans) on case trends.
