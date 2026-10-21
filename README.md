# ⚡ Electric Vehicle Market Analysis

### Exploring EV Specifications, Battery Performance, Driving Range & Vehicle Types

An exploratory data analysis project focused on understanding the technical specifications of electric vehicles (EVs) using Python, data visualization, and Tableau. This project transforms raw vehicle specification data into meaningful insights about battery capacity, driving range, energy efficiency, brand representation, and vehicle body types.

Live Dashboard: [Explore the Interactive Tableau Dashboard](https://public.tableau.com/app/profile/kanak.vishnoi/viz/ElectricVehicleMarketAnalysis_17925987403220/EVMarketAnalysisDashboard?publish=yes)

---

## 📌 Project Overview

Electric vehicles are an important part of the transition toward more sustainable transportation. Understanding their technical specifications can help users compare different models and explore the relationships between battery capacity, driving range, efficiency, and vehicle design.

This project analyzes an electric vehicle specification dataset containing 478 vehicle records. Python is used for data inspection, cleaning, exploratory analysis, and visualization, while Tableau is used to build an interactive dashboard.

The analysis focuses on identifying patterns in the available specifications rather than measuring actual vehicle sales or market share.

## 🎯 Project Objectives

- Analyze the representation of EV brands in the dataset.
- Explore the distribution of listed driving ranges.
- Investigate the relationship between battery capacity and driving range.
- Compare vehicle body types and drivetrain configurations.
- Prepare a cleaned dataset for reliable analysis.
- Build an interactive Tableau dashboard with KPIs and filters.
- Communicate findings through visualizations and documentation.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Data analysis and processing |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Tableau Public | Interactive dashboard and data exploration |
| CSV | Dataset storage and exchange |
| GitHub | Version control and project documentation |

## 📂 Project Structure

```text
EV-Market-Analysis/
│
├── inspect_data.py
├── clean_data.py
├── verify_cleaned_data.py
├── eda_analysis.py
├── ev_insights.py
│
├── outputs/
│   ├── ev_data_cleaned.csv
│   ├── ev_insights_report.txt
│   └── charts/
│       ├── top_10_brands.png
│       ├── ev_range_distribution.png
│       ├── battery_vs_range.png
│       └── ev_body_types.png
│
├── EV_Market_Analysis.twbx
└── README.md
```

Note: The workbook filename and folder structure above are examples. Keep the actual filenames that exist in your repository.

## 📊 Dataset Description

The dataset,"C:\Users\HP\Desktop\EVs-Market-Analysis\electric_vehicles_spec_2025.csv" , contains technical specifications for electric vehicle models.

Important fields include:

- `brand` and `model` — vehicle identification
- `battery_capacity_kWh` — listed battery capacity
- `range_km` — listed driving range
- `efficiency_wh_per_km` — listed energy consumption per kilometer
- `top_speed_kmh` — maximum listed speed
- `acceleration_0_100_s` — acceleration time from 0 to 100 km/h
- `fast_charging_power_kw_dc` — listed DC fast-charging power
- `drivetrain` — drivetrain configuration
- `car_body_type` — vehicle body type
- `seats` — seating capacity

The dataset is used for descriptive and exploratory analysis.

Data source: Add the original dataset download page or source URL here before submitting.

## 🧹 Data Collection & Preparation

The data preparation workflow includes:

1. Inspecting the dataset's dimensions, columns, data types, and missing values.
2. Checking for duplicate records.
3. Removing unnecessary leading and trailing whitespace from text fields.
4. Handling missing model names using an `Unknown` label.
5. Converting cargo-volume information into a numeric field where possible.
6. Preserving missing or unconvertible values rather than inventing values.
7. Exporting the prepared dataset to `outputs/ev_data_cleaned.csv`.
8. Verifying the cleaned dataset before visualization.

The cleaned dataset contains 478 records and 23 columns. The cleaning process does not remove vehicle records simply because some fields are missing.

## 📈 Exploratory Data Analysis

The project includes four main visualizations:

### 1. Top 10 EV Brands

Compares the number of listed vehicle records across the ten most represented brands in the dataset.

### 2. Driving Range Distribution

Shows how listed EV driving ranges are distributed across the available vehicle records.

### 3. Battery Capacity vs. Driving Range

Explores the relationship between battery capacity and listed driving range to identify patterns across different EV models.

### 4. EV Models by Body Type

Compares the number of records across vehicle body types, such as SUVs, sedans, and other available categories.

## 🔍 Key Findings

The exploratory analysis produced the following observations:

- 478 vehicle records are available in the cleaned dataset.
- SUVs are the most represented body type, with approximately 244 records.
- The average listed battery capacity is approximately 74.04 kWh.
- The average listed driving range is approximately 393.18 km.
- The average listed energy consumption is approximately 162.90 Wh/km.
- The maximum listed driving range is 685 km, associated with the Mercedes-Benz EQS 450+ in this dataset.
- Battery capacity and listed driving range have a Pearson correlation of approximately 0.88, indicating a strong positive linear association in the analyzed records.

These findings describe the available dataset and should not be interpreted as rankings of real-world sales, vehicle reliability, or actual on-road performance.

## 📊 Interactive Tableau Dashboard

The Tableau dashboard brings the analysis together in one place.

Dashboard features:
- KPI cards for total records, average driving range, and average battery capacity.
- Brand filter for exploring vehicle records.
- Drivetrain filter for comparing AWD, FWD, and RWD vehicles.
- Body type filter for exploring different vehicle categories.
- Four visualizations for comparing brands, range, battery capacity, and body types.

### 🚀 View the Live Dashboard

[Open Electric Vehicle Market Analysis on Tableau Public →](https://public.tableau.com/app/profile/kanak.vishnoi/viz/ElectricVehicleMarketAnalysis_17925987403220/EVMarketAnalysisDashboard?publish=yes)

## ▶️ How to Run the Python Analysis

### Prerequisites

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn

### Installation

Clone the repository:

```bash
 https://github.com/KanakVishnoi/EV-Market-Analysis/edit/main/README.md
```

Install the required packages:

```bash
pip install pandas numpy matplotlib seaborn
```

Place the original dataset in the expected project location and run the scripts in the following order:

```bash
python inspect_data.py
python clean_data.py
python verify_cleaned_data.py
python eda_analysis.py
python ev_insights.py
```

Make sure the input CSV path in the scripts matches your local folder structure.

## ⚠️ Limitations

- The dataset contains vehicle specifications, not actual sales or registration records.
- Brand counts represent the number of listed records in this dataset, not market share.
- Listed driving range may differ from real-world range because of driving conditions, temperature, speed, and other factors.
- Missing specification values may affect individual comparisons.
- The observed relationship between battery capacity and range does not establish causation.
- Findings depend on the completeness, consistency, and coverage of the available dataset.

## 🔮 Future Improvements

- Add more recent and diverse EV specification records.
- Compare specifications across vehicle segments and price ranges if reliable price data becomes available.
- Incorporate real-world range and charging-time measurements.
- Add source validation and automated data-quality checks.
- Improve dashboard interactions and add a structured Tableau Story.
- Expand the analysis with historical sales or registration data from reliable sources, if market trends are to be studied.

## 👩‍💻 Author

Kanak Vishnoi

B.Tech CSE — Artificial Intelligence & Machine Learning

Interested in Data Analytics, Machine Learning, and data-driven problem solving.

---

⭐ If you find this project useful, feel free to explore the dashboard and repository.

Built as a data analytics project to practice data preparation, exploratory data analysis, visualization, and interactive dashboard development.
