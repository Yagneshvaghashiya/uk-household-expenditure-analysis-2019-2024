# Data Dictionary

## Dataset Overview

**Source:** Office for National Statistics (ONS)  
**Time Period:** 2019-2024  
**Frequency:** Annual  
**Unit of Measurement:** Average weekly spending per household (£)

## Main Dataset

**File:** `data/Main_File_Compile_All_Data_Year_from_2019_to_2024_Expenditure.xlsx`

### Column Descriptions

| Column Name | Data Type | Description | Example |
|------------|-----------|-------------|---------|
| Year | Integer | Financial year ending (e.g., 2019 = Apr 2018 - Mar 2019) | 2019, 2020, 2021 |
| Category | Text | Expenditure category name | "Food & non-alcoholic drinks" |
| Spend | Decimal | Average weekly household expenditure in £ | 62.40 |
| COVID_Period | Text | Classification of pandemic period | "Pre-COVID", "During-COVID", "Post-COVID" |

### Expenditure Categories

#### 1. **All expenditure groups**
- Total household spending across all categories

#### 2. **Food & non-alcoholic drinks**
- Bread and cereals
- Meat, fish
- Dairy products
- Fruit and vegetables
- Non-alcoholic beverages

#### 3. **Alcoholic drink, tobacco & narcotics**
- Alcoholic beverages
- Tobacco
- Narcotics

#### 4. **Clothing & footwear**
- Clothing materials
- Garments
- Footwear
- Cleaning and repair

#### 5. **Housing, fuel & power**
- Rent payments
- Mortgage payments
- Council tax
- Electricity, gas
- Water supply

#### 6. **Household goods & services**
- Furniture and furnishings
- Household textiles
- Household appliances
- Glassware, tableware
- Household services

#### 7. **Health**
- Medical products
- Out-patient services
- Hospital services

#### 8. **Transport**
- Purchase of vehicles
- Operation of personal transport
- Transport services
- Public transport

#### 9. **Communication**
- Postal services
- Telephone and telefax equipment
- Telephone and telefax services

#### 10. **Recreation & culture**
- Audio-visual equipment
- Sports equipment
- Cultural services
- Package holidays
- Books, newspapers

#### 11. **Education**
- Pre-primary and primary education
- Secondary education
- Tertiary education

#### 12. **Restaurants & hotels**
- Catering services
- Accommodation services

#### 13. **Miscellaneous goods & services**
- Personal care
- Personal effects
- Social protection
- Insurance
- Financial services

## COVID Period Classifications

| Period | Years | Description |
|--------|-------|-------------|
| Pre-COVID | 2019 | Normal economic conditions before pandemic |
| During-COVID | 2020-2021 | Pandemic period with lockdowns and restrictions |
| Post-COVID | 2022-2024 | Recovery and adaptation period |

## Raw Data Files

Located in `raw_data/` folder:

### Technical Reports (Tables)
- `ok_techreport201819tablesfinalised1.xls` - 2018-2019 data
- `ok_technicalreport201920tables__1_.xls` - 2019-2020 data
- `ok_technicalreport202021tables.xls` - 2020-2021 data
- `ok_technicalreport202122tablesfinal.xlsx` - 2021-2022 data
- `ok_technicalreport202223tables.xlsx` - 2022-2023 data

### Workbooks (Detailed Expenditure)
- `ok_familyspendingworkbook1detailedexpenditureandtrends.xlsx` - Multi-year trends
- `ok_workbook1detailedexpenditureandtrends_Year_Ending_2021.xlsx` - 2021 specific
- `ok__Year_Ending_2024.xlsx` - 2024 data

## Data Quality Notes

### Missing Data
- No significant missing values in core categories
- Some minor categories may have suppressed values due to low sample size

### Data Transformations
1. **Unpivoting:** Wide format (years as columns) → Long format (years as rows)
2. **Type conversion:** Year converted from text to integer
3. **Calculated columns:** COVID_Period classification added
4. **Aggregation:** Weekly averages maintained as per ONS methodology

### Known Limitations
- Data represents average household spending
- May not reflect extremes (very high/low income households)
- Regional variations are not captured in this analysis
- Sampling error margins not included

## Measurement Units

- **Currency:** British Pounds (£)
- **Time Period:** Weekly averages
- **Sample Unit:** Household

## Data Collection Methodology

Sourced from the ONS Living Costs and Food Survey (LCF):
- Sample size: ~5,000 households per year
- Collection method: Diary-based survey
- Duration: 14-day diary keeping period
- Coverage: United Kingdom

## Updates and Versions

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | Dec 2025 | Initial compiled dataset for academic analysis |

## References

For detailed methodology:
- [ONS Family Spending Methodology](https://www.ons.gov.uk/peoplepopulationandcommunity/personalandhouseholdfinances/expenditure/methodologies/familyspendingsurveyandexpenditureandincomesurveyqmi)
- [Living Costs and Food Survey User Guide](https://www.ons.gov.uk/peoplepopulationandcommunity/personalandhouseholdfinances/incomeandwealth/methodologies/livingcostsandfoodsurveytechnicalreportfinancialyearending2020)

## Contact for Data Questions

**Project Author:** Yagnesh Vaghashiya  
**Institution:** London Metropolitan University  
**Data Source:** Office for National Statistics (ONS)  
**Data Queries:** contact.ons.gov.uk
