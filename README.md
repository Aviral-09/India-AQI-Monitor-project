# India AQI Analyzer 🇮🇳

A Python project to fetch, analyze, and visualize real-time Air Quality Index (AQI) data for Indian cities using the Open-Meteo Air Quality API.

## Features
- **Real-time Data**: Fetches PM2.5, PM10, NO2, O3, SO2, and CO levels.
- **Comprehensive Coverage**: Includes a dataset of major Indian cities.
- **CLI Tool**: Batch fetch data for all cities and save to CSV.
- **Interactive Dashboard**: Streamlit-based UI for visualization and analysis.
- **AQI Categorization**: Automatically categorizes air quality (Good, Moderate, Poor, etc.).

## Project Structure
```
India_AQI_Analyzer/
├── aqi_api.py             # API integration module
├── city_loader.py         # City data loader
├── utils.py               # Helper functions (AQI logic)
├── app.py                 # CLI application
├── dashboard.py           # Streamlit dashboard
├── India_Cities.csv       # Input dataset
├── India_All_Cities_AQI.csv # Output dataset (generated)
└── README.md              # Documentation
```

## Installation

1. Clone or download the repository.
2. Install dependencies:
   ```bash
   pip install pandas requests streamlit plotly
   ```

## Usage

### 1. CLI Mode (Batch Processing)
Run the script to fetch data for all cities and generate the report.
```bash
python app.py
```
- This will create `India_All_Cities_AQI.csv`.
- It will also print the Top 10 Most Polluted and Cleanest cities to the console.

### 2. Dashboard Mode (Interactive UI)
Launch the Streamlit dashboard.
```bash
streamlit run dashboard.py
```
- View real-time data for specific cities.
- Compare cities using interactive charts.
- View the full dataset.

## API Used
- **Open-Meteo Air Quality API**: [https://open-meteo.com/en/docs/air-quality-api](https://open-meteo.com/en/docs/air-quality-api)
- No API key required for non-commercial use.

## License
Open Source.
