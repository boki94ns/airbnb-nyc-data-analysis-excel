# NYC Airbnb Listings: Exploratory Data Analysis in Excel

**Data Analytics Portfolio Project | Coders Lab**

## 📥 Excel Project — View & Download

**[📊 CLICK HERE TO OPEN THE COMPLETE EXCEL ANALYSIS](airbnb_recruitment_task.xlsx)**

The link above opens the original Excel workbook in this GitHub repository. Use GitHub's **Download raw file** option to download it and open it in Microsoft Excel. The complete dataset, formulas, PivotTables, and worksheets are in that file; a full interactive Excel worksheet cannot be embedded directly into a GitHub README.

| Project file | What it contains | Access |
| --- | --- | --- |
| `airbnb_recruitment_task.xlsx` | 39,881 NYC Airbnb listings, calculations, descriptive statistics and PivotTables | **[Open / download Excel workbook](airbnb_recruitment_task.xlsx)** |
| `README.md` | Project description, questions, methods and key results | You're reading it |

## Project Overview

This project explores New York City Airbnb listing data using Microsoft Excel. It uses descriptive statistics, calculated categories, PivotTables, and chart-based summaries to investigate pricing, room types, neighbourhoods, hosting activity, and minimum-stay requirements.

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
- **Additional coursework (not uploaded here):** scatter charts with two linear trendlines and one polynomial trendline were created for separate presentations. These were exploratory visualisations, not a predictive machine-learning model.

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

## Dataset Columns at a Glance

The workbook contains the following fields, among others:

| Column | Description |
| --- | --- |
| `neighbourhood_group` | NYC borough |
| `neighbourhood` | Neighbourhood where the listing is located |
| `room_type` | Type of accommodation offered |
| `price` | Listed accommodation price |
| `minimum_nights` | Minimum required stay |
| `number_of_reviews` | Recorded number of reviews |
| `availability_365` | Listed availability over 365 days |
| `price_range` | Calculated price category |
| `rental_duration` | Calculated short-, mid-, or long-term category |

**To see all 39,881 records, open the [full Excel workbook](airbnb_recruitment_task.xlsx).** The tables in this README are concise summaries rather than a duplicate of the full dataset.

## Repository Files

```text
airbnb-nyc-data-analysis-excel/
├── README.md
└── airbnb_recruitment_task.xlsx
```

The workbook is the primary deliverable. It contains the actual analysis and is directly accessible from the link above.

## Limitations

- This is an educational, descriptive analysis of the supplied dataset; the collection period and data-source licence are not specified in the workbook.
- Observed patterns describe associations, not proven causes or validated forecasts. Regression-related exploration was documented separately during the course; the Excel workbook linked here is the file published in this repository.
- The full Excel workbook remains the primary source for formulas and detailed calculations.

## Author

**Bojan Milić**  
Aspiring Data Scientist | Data Analytics | Novi Sad, Serbia
