# NYC Airbnb Listings: Exploratory Data Analysis in Excel

**Data Analytics Portfolio Project | Coders Lab**

## Project Overview

This project explores New York City Airbnb listing data using Microsoft Excel. It combines descriptive statistics, calculated categories, PivotTables, charts, and exploratory regression trendlines to investigate pricing, room types, neighbourhoods, hosting activity, and minimum-stay requirements.

The workbook contains **39,881 listings** across New York City's five boroughs, with **17 columns** including listing and host identifiers, location, room type, listed price, minimum nights, reviews, and availability. This is an **exploratory analysis** project, not a production pricing model.

## Questions Explored

- What types of Airbnb accommodation are most common?
- Which neighbourhoods contain the most listings?
- How do average listing prices differ between neighbourhoods and room types?
- Are listings more commonly offered for short-, medium-, or long-term stays?
- What is the distribution of minimum-night requirements?
- What relationships can be visualised between minimum nights, prices, and reviews?

## Dataset and Workbook Structure

The main dataset is in `airbnb_recruitment_task.xlsx`. It includes:

| Worksheet | Contents |
| --- | --- |
| `airbnb_recruitment_task` | Listing-level dataset, price-category formulas, and rental-duration classification |
| `NULL_provera` | Record-count checks across dataset fields |
| `EDA` | Descriptive statistics and counts of unique values |
| `EDA_pivot_tables` | PivotTables for room types, neighbourhoods, prices, and related breakdowns |
| `EDA_pivot_tables2` | Additional PivotTables for minimum nights, host listings, and neighbourhood-level metrics |
| `Communication` | Aggregated results prepared for communication and presentation |
| `IN_DEPTH` | A worksheet reserved for deeper analysis; the regression charts are in the presentations |

**Dataset variables:** `id`, `name`, `host_id`, `host_name`, `neighbourhood_group`, `neighbourhood`, `room_type`, `price`, `price_range`, `minimum_nights`, `rental_duration`, `number_of_reviews`, `last_review`, `reviews_per_month`, `calculated_host_listings_count`, `availability_365`, and `number_of_reviews_ltm`.

## Tools and Methods

**Microsoft Excel**

- **Descriptive statistics:** `MIN`, `MAX`, `AVERAGE`, and `MEDIAN` for numeric variables.
- **Distinct-count analysis:** `UNIQUE` and `COUNTA` to examine hosts, neighbourhoods, and room types.
- **Calculated categories:** nested `IF` formulas, `MEDIAN`, and `PERCENTILE.INC` to group listing prices into `CHEAP`, `NORMAL`, and `EXPENSIVE`.
- **Rental-duration classification:** nested `IF` formulas based on `minimum_nights`:
  - **Short-term:** fewer than 14 nights
  - **Mid-term:** 14–30 nights
  - **Long-term:** more than 30 nights
- **Data validation:** record-count checks for the analysed fields.
- **PivotTables and charts:** comparisons across room types, boroughs, neighbourhoods, minimum-night requirements, reviews, host listings, and prices.
- **Exploratory regression visualisation:** two linear trendlines and one polynomial trendline added to scatter charts; used to explore associations, not to establish causation or build a predictive machine-learning model.

## Selected Findings

| Metric | Result |
| --- | ---: |
| Airbnb listings analysed | 39,881 |
| Distinct host IDs | 26,292 |
| Distinct neighbourhoods | 244 |
| Mean listed price | 197.70 |
| Median listed price | 130.00 |
| Entire home/apartment listings | 22,761 (57.1%) |
| Private-room listings | 16,361 (41.0%) |
| Short-term listings | 19,676 (49.3%) |
| Mid-term listings | 18,315 (45.9%) |
| Long-term listings | 1,890 (4.7%) |

**Location and listing mix**

- Manhattan contains **16,847** listings, followed by Brooklyn with **14,845** and Queens with **6,175**.
- The most frequently represented neighbourhoods are **Bedford-Stuyvesant** (2,779 listings), **Williamsburg** (2,456), and **Harlem** (1,878).
- Entire homes/apartments are the most common room type, followed by private rooms.
- Listings classified as short-term have a slight lead over those classified as mid-term, while long-term listings are comparatively uncommon.

**Pricing observations**

- The mean listed price (**197.70**) is higher than the median (**130.00**), consistent with a right-skewed price distribution influenced by higher-priced listings.
- The dataset includes high price outliers; averages for individual neighbourhoods should therefore be considered alongside sample sizes and other distribution measures.
- Price categories are defined by thresholds from the dataset, rather than independently validated market standards.

## Presentation Materials

The project also includes three compact versions of the original PowerPoint presentations. Their **chart visuals and cached data are retained** for viewing, but their large embedded Excel workbooks were removed to make browser upload practical. Use the main `.xlsx` file to inspect and edit the actual analysis.

1. [EDA Results Presentation](airbnb_eda_results.pptx) — room types, neighbourhood prices, nightly price comparisons, listing counts, and rental-duration categories.
2. [Communication Results](airbnb_communication_results.pptx) — key insights for an audience: property types, listings by neighbourhood, price differences, stay length, and minimum-night distributions.
3. [In-Depth Regression Analysis](airbnb_regression_analysis.pptx) — scatter plots with linear trendlines for minimum nights vs. price and review counts vs. monthly reviews, plus a polynomial trendline for minimum nights vs. review counts.

## Repository Files

```text
airbnb-nyc-data-analysis-excel/
├── README.md
├── airbnb_recruitment_task.xlsx
├── airbnb_eda_results.pptx
├── airbnb_communication_results.pptx
└── airbnb_regression_analysis.pptx
```

## Limitations

- This is an educational, descriptive analysis of the supplied dataset; the collection period and data-source licence are not specified in the workbook.
- Observed patterns and regression trendlines describe associations only. They should not be treated as causal explanations or validated forecasts.
- The full Excel workbook remains the primary source for formulas and detailed calculations.

## Author

**Bojan Milić**  
Aspiring Data Scientist | Data Analytics | Novi Sad, Serbia
