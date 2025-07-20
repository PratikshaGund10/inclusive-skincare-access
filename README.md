# Inclusive Skincare Access: A Geo-Demographic Micromarketing Project

This project uses data science, spatial analytics, and micromarketing to identify and prioritize outreach opportunities for inclusive skincare access among **Hispanic women aged 15–44**—a fast-growing, underrepresented demographic in the wellness space.

The initiative is built in phases, from high-level geographic targeting to trade area identification, lifestyle segmentation, and expansion modeling. Each phase combines real data with community-centered decision-making to drive impact where it matters most.

_Last updated: July 20, 2025_

---

## 🗂️ Project Workflow Overview

| Phase | Description | Status |
|-------|-------------|--------|
| ✅ Phase 1 | State Selection — Based on population concentration and skincare spending | Complete |
| ✅ Phase 2 | ZIP-to-County Aggregation — Identify top counties in New Mexico | Complete |
| ✅ Phase 3 | Trade Area Definition — Identify high-potential block groups | Complete |
| ✅ Phase 4 | Retail Partner Selection & Buyer Estimation | Complete |
| ✅ Phase 5 | Lifestyle Segmentation — Understand who lives there and how they shop | Complete |
| ✅ Phase 6 | Expansion Modeling — Locate lookalike trade areas | Complete |

---

## 🔧 Tools & Data Sources

- **Alteryx Designer** — For data prep, spatial analytics, enrichment, segmentation
- **ArcGIS Pro** — For geospatial analysis and trade area visualization
- **Esri Demographics (2024)** — Age, race, spending, lifestyle segments
- **U.S. Census / FIPS / ZIP shapefiles**
- **ParseHub + Yellow Pages** — Web scraping for retail locations

---

## 📍 Phase 1: State Selection Using Demographic and Spending Data

**Goal:** Identify the U.S. state where skincare outreach to Hispanic women aged 15–44 can have the highest impact.

### Alteryx Formulas

- **Raw Count (HISP1545)**  
  ![](assets/alteryx_formula_sum_hispanic_females_15_44.png)

- **Percent of Population (HISPp1545)**  
  ![](assets/alteryx_formula_percent_hispanic_females_15_44.png)

---

### Output: State-Level Summary  
![](assets/alteryx_output_state_selection_hispanic_spend.png)

**New Mexico selected** due to:
- Highest % of Hispanic females aged 15–44 (10.29%)
- Strong raw count (219,000+)
- Moderate but significant skincare spend ($210.74 per household)

---

## 📍 Phase 2: ZIP-to-County Aggregation

**Goal:** Identify New Mexico counties with the highest opportunity for outreach.

### Alteryx Workflows  
![](assets/alteryx_workflow_zipcode_enrichment_and_county_join.png)  
![](assets/alteryx_summarize_groupby_county_metrics.png)

---

### Output Table  
![](assets/zip_level_enrichment_table.png)

### County Rankings  
- **Bernalillo County**: 74,602 women in target group  
- **Dona Ana County**: Highest % (15.51%)  
![](assets/alteryx_sort_county_by_usergroup_percentage.png)  
![](assets/alteryx_sort_counties_by_total_target_group.png)

---

## 📍 Phase 3: Trade Area Definition

**Goal:** Identify block groups with ≥280 Hispanic females aged 15–44 using Esri & census data.

### Threshold Calculation  
![](assets/alteryx_profile_statistics_hisp1545_threshold.png)

### Filtered Block Groups  
![](assets/alteryx_map_and_workflow_filtered_trade_areas.png)

---

### ZIP Focus Map (87121)  
![](assets/arcgis_trade_area_map_target_zip_87121.png)  
![](assets/arcgis_trade_area_map_legend.png)

---

## 📍 Phase 4: Retail Partner Selection & Buyer Estimation

**Goal:** Select best retail hub in ZIP 87121 using spend, reach, and user-group density.

### Workflow & Store Comparison  
![](assets/alteryx_workflow_beauty_retailer_addresses_87121.png)  
![](assets/arcgis_trade_area_map_remove_overlap_87121.png)  
![](assets/alteryx_trade_area_comparison_87121.png)

---

### Buyer Estimations  
- **Total Buyers (based on $1,000/yr spend):**  
  ![](assets/alteryx_estimate_total_buyers_sunficent.png)

- **Target Group Buyers (Hispanic females 15–44):**  
  ![](assets/alteryx_estimate_target_group_reach_sunficent.png)

---

## 📍 Phase 5: Lifestyle Segmentation – Behavioral Targeting

**Goal:** Understand the dominant lifestyle segments in our best-performing trade area.

### Map: Esri Tapestry Segments  
![](assets/arcgis_tapestry_segments_trade_area_sunficent.png)

### Alteryx Workflow  
![](assets/alteryx_workflow_enriched_trade_area_segmentation.png)

---

### Segment Breakdown

| Segment | Households | % of Total |
|---------|------------|------------|
| 7A: Up and Coming Families | 3,178 | 43.4% |
| 8C: Bright Young Professionals | 1,080 | 14.8% |
| 4A: Workday Drive | 1,077 | 14.7% |
| 4B: Home Improvement | 718 | 9.8% |
| 8E: Front Porch | 512 | 7.0% |
| 11C: Metro Fusion | 558 | 7.6% |

![](assets/alteryx_tapestry_segmentation_output_sunficent.png)  
![](assets/alteryx_tapestry_segmentation_percentages_sunficent.png)

---

### Segment Profile: 7A – Up and Coming Families

![](assets/tapestry_7A_summary_traits.png)  
![](assets/tapestry_7A_demographics_spending.png)  
![](assets/tapestry_7A_market_profile_indices.png)

---

## 📍 Phase 6: Expansion Modeling – Identifying Lookalike Trade Areas

**Goal:** Identify new skincare retail sites in nearby ZIPs that also attract high-density 7A populations.

---

### Step 1: Scrape Nearby Cosmetic Stores

![](assets/parsehub_scrape_yellowpages_cosmetics_87120.png)

> Extracted skincare/cosmetic stores near ZIP 87120 using ParseHub + Yellow Pages for trade area testing.

---

### Step 2: Clean and Parse Address Data

![](assets/alteryx_cleaning_scraped_addresses_87120.png)

---

### Step 3: Trade Area Evaluation by 7A Households

![](assets/alteryx_trade_area_comparison_7A_expansion.png)

> **Top Expansion Site: Paseo del Norte NW**  
> - 1,369 households in 7A (81.54%)  
> - Higher concentration than Sunficent LLC (833, 38.37%)  
> - Old Coors Dr SW less promising (30 households, 2.48%)

---

## 💬 Final Thoughts

This project models how micromarketing + spatial analysis can power **inclusive wellness outreach** using real demographic and consumer behavior data.

The final phase will explore **campaign modeling and impact estimation** for each selected area.

---

## 👤 Author

**Pratiksha Gund**  
📍 Data Analyst | Micromarketing Researcher  
🔗 [LinkedIn] (https://www.linkedin.com/in/pratiksha-gund/) | 🌐 [Portfolio] | ✉️ [Email] (pratikshagund10@gmail.com)

---

## 🏷 Tags

#Micromarketing #GIS #RetailAnalytics #Alteryx #ArcGIS #DataForGood #ConsumerInsights #InclusiveSkincare #BehavioralTargeting #TradeAreaModeling
