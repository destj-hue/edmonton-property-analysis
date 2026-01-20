# Edmonton Residential Property Value Analysis

A comprehensive data analysis project examining residential property assessment patterns across Edmonton, Alberta using Python and interactive visualizations.

## Project Overview

This project analyzes over 400,000 residential property records from the City of Edmonton's Open Data portal to identify key factors influencing property values, geographic patterns in pricing, and market segmentation across neighborhoods.

## Key Features

- Statistical analysis of 400,000+ property assessment records
- Correlation analysis identifying key drivers of property values
- Interactive visualizations using Bokeh
- Geographic mapping of property value distributions
- Neighborhood and ward-level comparative analysis
- Market segmentation by property value brackets

## Technologies Used

- **Python 3.x** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Bokeh** - Interactive data visualization
- **Google Colab** - Development environment

## Dataset

**Source:** [City of Edmonton Open Data Portal](https://data.edmonton.ca/City-Administration/Property-Assessment-Data-Current-Calendar-Year-/q7d6-ambg/about_data)

**Records:** 400,000+ residential properties  
**Year:** 2025  
**Format:** Excel (.xlsx) / CSV

## Key Findings

- **Mean residential property value:** $370,925.80 
- **Median residential property value:** $367,500.00
- **Most expensive neighborhoods:** Heritage Valley, Mistatim Industrial, and Goodridge Corners
- **Strongest value correlations:** None from this dataset

## Analyses Performed

### 1. Descriptive Statistics
- Mean, median, standard deviation of assessed values
- Quartiles and percentiles
- Min/max value identification

### 2. Correlation Analysis
- Identified no factors correlated with property values in this dataset

### 3. Geographic Analysis
- Average values by neighborhood
- Average values by municipal ward
- Most and least expensive areas

### 4. Market Segmentation
- Property value brackets (<$200K, $200K-400K, $400K-600K, etc.)
- Distribution analysis across brackets

## Visualizations

The project includes 7+ interactive visualizations:

1. **Distribution Histogram** - Property value frequency distribution
2. **Neighborhood Bar Chart** - Top 20 neighborhoods by average value
3. **Ward Bar Chart** - Top 5 wards by average value
4. **Correlation Chart** - Factors most strongly correlated with value
5. **Geographic Heatmap** - Spatial distribution of property values
6. **Interactive Map** - Explore properties across Edmonton

## Installation & Usage

### Prerequisites
```bash
Python 3.x
pandas
numpy
bokeh
```

### Running the Analysis

1. **Clone the repository:**
```bash
git clone https://github.com/destj-hue/edmonton-property-analysis.git
cd edmonton-property-analysis
```

2. **Open in Google Colab:**
- Upload `YEG_Property_Assessments.ipynb` to Google Colab
- Or click: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/destj-hue/edmonton-property-analysis/blob/main/YEG_Property_Assessments.ipynb)

3. **Download the dataset:**
- Visit [Edmonton Open Data Portal](https://data.edmonton.ca/City-Administration/Property-Assessment-Data-Current-Calendar-Year-/q7d6-ambg/about_data)
- Export as Excel or CSV
- Upload to your Colab environment

4. **Run the notebook:**
- Execute cells sequentially from top to bottom
- Interactive visualizations will display inline

## Project Structure
```
edmonton-property-analysis/
│
├── YEG_Property_Assessments.ipynb    # Main analysis notebook
├── README.md                          # Project documentation
├── edmonton_property_map_bokeh.html  # Interactive map visualization
├── edmonton_properties.json          # Exported data
└── requirements.txt                   # Python dependencies (optional)
```

## Data Cleaning Process

1. **Column standardization** - Identified and renamed key columns
2. **Missing value handling** - Removed records with missing assessed values
3. **Outlier removal** - Filtered properties with $0 or negative assessments
4. **Type filtering** - Isolated residential properties using Tax Class field
5. **Data type conversion** - Converted numeric fields from strings to numbers

## Results Summary

### Statistical Insights
- Comprehensive descriptive statistics for residential properties
- Identified distribution patterns across value ranges
- Quantified variability in property values across neighborhoods

### Geographic Insights
- Mapped high-value and low-value neighborhood clusters
- Identified ward-level pricing patterns
- Visualized spatial distribution of property values

## Challenges & Solutions

**Challenge:** Dataset contained mixed property types (residential, commercial, industrial)  
**Solution:** Filtered to residential properties only using Tax Class field

**Challenge:** Large dataset (400,000+ records) impacted visualization performance  
**Solution:** Applied strategic sampling for geographic visualizations

## Future Enhancements

- [ ] Time-series analysis comparing multiple years
- [ ] Predictive modeling for property value estimation
- [ ] Integration of demographic data (schools, transit, amenities)
- [ ] Determination of the data that strongly correlates with assessed property value
- [ ] Machine learning classification of neighborhood tiers
- [ ] Automated dashboard with real-time data updates

## Skills Demonstrated

- Large-scale data processing and cleaning
- Statistical analysis and interpretation
- Correlation and relationship analysis
- Interactive data visualization
- Geospatial data analysis
- Python programming (pandas, NumPy, Bokeh)
- Problem-solving and debugging
- Documentation and code organization

## Author

**Destanee Charrois**  
[Your LinkedIn](https://www.linkedin.com/in/destanee-charrois-776aa0a2/) | [Your Portfolio](https://www.humandesignhub.ca/portfolio) 


## Acknowledgments

- City of Edmonton for providing open access to property assessment data
- [M2M Tech DataTalent Program] (https://m2mtechconnect.com/programs/datatalent) for project guidance and support

## Contact

For questions or collaboration opportunities, please reach out via LinkedIn

---

**Note:** This project was completed as part of a data analysis capstone. The analysis is for educational and portfolio purposes. Property values are based on official assessment data and may not reflect current market prices.

