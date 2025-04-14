# Bangladesh Garment Industry Analysis

![Garment Factory Map](images/factory_map.png)

## Project Overview
This project analyzes data from the Bangladesh Garment Manufacturers and Exporters Association (BGMEA) to provide insights into the country's ready-made garment (RMG) industry - the backbone of Bangladesh's economy, contributing over 80% of export earnings.

## Key Features
- **Geospatial Analysis**: Factory distribution mapping
- **Capacity Benchmarking**: Production capability assessment
- **Efficiency Metrics**: Machine and labor productivity analysis
- **Predictive Modeling**: Capacity forecasting models
- **Business Intelligence**: ROI calculators and risk dashboards

## Dataset
The dataset contains information on 1,000+ BGMEA-listed garment factories with:
- Factory characteristics (type, size, age)
- Production capacity metrics
- Workforce and machine data
- Geographic locations
- Product specializations

## Project Structure
bgmea-analysis/
├── data/
│ ├── raw/ # Original data files
│ └── processed/ # Cleaned and enhanced data
├── notebooks/
│ ├── 1_data_cleaning.ipynb
│ ├── 2_eda.ipynb # Exploratory Data Analysis
│ ├── 3_modeling.ipynb # Predictive models
│ └── 4_business_insights.ipynb
├── src/
│ ├── geocoding.py # Location processing
│ └── visualization.py # Plot utilities
├── reports/
│ ├── figures/ # Saved visualizations
│ └── insights.md # Key findings
└── app/ # Interactive dashboard

Copy

## Key Analyses
1. **Factory Clustering**
   - Grouped factories by characteristics using K-means
   - Validated with silhouette scores (0.62) and Davies-Bouldin index (0.85)

2. **Capacity Prediction**
   - Random Forest model achieves R² = 0.87
   - Key predictors: Machine count, factory type, product diversity

3. **Risk Assessment**
   - Identified 68% capacity concentration in Gazipur-Dhaka cluster
   - 45% of factories specialize in only 3 product types

## Usage

### Requirements
- Python 3.8+
- Jupyter Notebook
- Key packages: pandas, scikit-learn, plotly, dash, folium

### Installation
```bash
git clone https://github.com/yourusername/bangladesh-garment-analysis.git
cd bangladesh-garment-analysis
pip install -r requirements.txt
Running Analyses
Start Jupyter Notebook:

bash
Copy
jupyter notebook
Execute notebooks in order:

Data Cleaning → EDA → Modeling → Business Insights

Launch Dashboard:

bash
Copy
python app/dashboard.py
Access at: http://localhost:8050

Key Findings
Top Performing Cluster: Cluster 2 (Narayanganj) shows 28% higher efficiency

Upgrade ROI: Knit factories in Gazipur offer best 3-year ROI (142%)

Risk Factors: Over-reliance on woven products in Dhaka cluster

Recommendations
For Factories:

Target 15-20% capacity increase through machine upgrades

Diversify into 2-3 additional product categories

For Policymakers:

Incentivize factories in underutilized regions

Support skill development for sweater production

For Buyers:

Source woven products from Cluster 1 (Dhaka)

Partner with Cluster 0 (Gazipur) for knitwear

