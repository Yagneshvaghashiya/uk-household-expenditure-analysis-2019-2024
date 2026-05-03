# UK Household Expenditure Analysis (2019-2024)

## 📊 Project Overview

A comprehensive time series analysis of UK household spending patterns before, during, and after the COVID-19 pandemic. This project analyzes expenditure data from 2019 to 2024 to identify trends, structural changes, and economic impacts on consumer behavior.

**Student:** Yagnesh Vaghashiya
**Institution:** London Metropolitan University  
**Supervisor:** Dr. Subeksha Shrestha

## 🎯 Research Question

*How did household spending patterns in the United Kingdom change before and after the COVID-19 pandemic (2019–2024)?*

## 🔍 Key Findings

- **Essential spending** (housing, food, transport) remained relatively stable throughout the pandemic
- **Non-essential spending** (recreation, culture, hospitality) showed significant volatility during economic disruptions
- Clear pre-pandemic, pandemic, and post-pandemic spending patterns identified
- Household adaptability demonstrated through spending reallocation strategies

## 📁 Project Structure

```
household-expenditure-analysis/
├── data/                          # Processed and compiled datasets
│   └── Main_File_Compile_All_Data_Year_from_2019_to_2024_Expenditure.xlsx
├── raw_data/                      # Original ONS data files (2018-2024)
│   ├── ok_technicalreport*.xls(x)
│   └── ok_workbook*.xlsx
├── powerbi/                       # Power BI dashboard files
│   └── Household_Expenses_Over_2019-2024.pbix
├── reports/                       # Academic reports and documentation
│   ├── A_Time_Series_Analysis_of_Household_Expenditure_Patterns.pdf
`

## 📊 Analytical Model

**Time Series Analysis** was selected as the primary analytical approach because it:
- Identifies long-term trends and patterns
- Captures seasonality and cyclical behavior
- Enables pre/post-pandemic comparison
- Reveals structural breaks caused by major events (COVID-19)

## 🗂️ Data Sources

All data sourced from the **Office for National Statistics (ONS)**:
- [Family Spending in the UK](https://www.ons.gov.uk/peoplepopulationandcommunity/personalandhouseholdfinances/expenditure/bulletins/familyspendingintheuk/april2023tomarch2024)
- [Living Costs and Food Survey Technical Reports](https://www.ons.gov.uk/peoplepopulationandcommunity/personalandhouseholdfinances/expenditure/datasets/livingcostsandfoodsurveytechnicalreportdatatables)

### Key Variables Analyzed:
- Food and non-alcoholic drinks
- Housing, fuel and power
- Transport
- Recreation and culture
- Restaurants and hotels
- Clothing and footwear
- Communication
- Education
- Health

## 🛠️ Tools & Technologies

- **Data Cleaning & Transformation:** Power Query (Power BI)
- **Data Analysis:** Time series methods, trend analysis, YoY comparisons
- **Visualization:** Power BI Desktop
- **Reporting:** Academic journal format (IEEE referencing style)
- **Data Processing:** Microsoft Excel

## 📈 Methodology

Following the **Data Analytical Life Cycle**:

1. **Discover:** Define research objectives and scope
2. **Data Preparation:** Clean, transform, and consolidate multi-year ONS data
3. **Plan Model:** Select time series analysis approach
4. **Build Model:** Create DAX measures, categorize COVID periods, analyze trends
5. **Communicate:** Develop interactive Power BI dashboards
6. **Measure Effectiveness:** Validate findings against literature and peer review

## 📊 Key Visualizations

The Power BI dashboard includes:
- **Time-series line charts** showing expenditure trends across all categories (2019-2024)
- **Category comparison bar charts** highlighting spending distribution
- **Year-over-year analysis** with COVID period segmentation
- **Interactive filters** by year, category, and COVID period
- **KPI cards** displaying total spending and key metrics

## 🎓 Academic Contributions

This analysis contributes to:
- Understanding consumer behavior during economic crises
- Policy development for household financial support
- Economic recovery planning post-pandemic
- Longitudinal analysis combining time-series and visual analytics

## 📝 Key References

1. Office for National Statistics (ONS). (2020). *Family Spending in the UK: April 2019 to March 2020*
2. Box, G.E.P., Jenkins, G.M., & Reinsel, G.C. (2008). *Time Series Analysis: Forecasting and Control*
3. Madudova, E., & Corejova, T. (2024). *The Issue of Measuring Household Consumption Expenditure*. Economies, 12(1), 9
4. McKibbin, W., & Fernando, R. (2023). *The Global Economic Impacts of the COVID-19 Pandemic*. Economic Modelling

## 📊 Dashboard Preview

The interactive dashboard features:
- **Total spending:** 9K (sum of all categories)
- **Filters:** Year, Category, COVID Period
- **Trend visualization:** Multi-category time series
- **Category breakdown:** Bar chart comparison

## 🔄 Future Work

Potential extensions:
- Monthly granularity analysis
- Forecasting models (ARIMA/SARIMA)
- Regional breakdown of spending patterns
- Automated anomaly detection
- Scenario testing for future economic shocks

## 💡 Practical Implications

### For Policymakers:
- Essential expenditure stability suggests targeted support programs work
- Non-essential sector volatility indicates need for flexible stimulus measures

### For Households:
- Importance of flexible budgeting
- Prioritization of essential spending during uncertainty
- Room for non-essential spending in stable economic conditions

## 📞 Contact

**Yagnesh Vaghashiya**  
Mail ID: yagneshvaghashiya602@gmail.com
Mobile Number: +44 7887 172884

## 📄 License

This project is submitted as academic coursework for CC7183 Data Analysis and Visualisation. All data is sourced from publicly available ONS datasets. Please cite this work if used for academic purposes.

## ⚠️ Academic Integrity

This work complies with London Metropolitan University's academic integrity policy. All datasets, code, and literature are properly referenced following IEEE style guidelines.

---

*Last Updated: December 2025*
