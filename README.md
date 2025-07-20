# Inclusive Skincare Access: A Geo-Demographic Micromarketing Project

This project uses data science, spatial analytics, and micromarketing to identify and prioritize outreach opportunities for **inclusive skincare access** among **Hispanic women aged 15–44**—a fast-growing, underrepresented demographic in the wellness space.

Each phase is grounded in real data and business logic, designed to be scalable, replicable, and community-driven. This project not only empowers equitable access to wellness but also models how brands can achieve **targeted growth** while driving **social impact**.

---

## 🗂️ Project Workflow Overview

| Phase | Description | Why It Matters |
|-------|-------------|----------------|
| ✅ Phase 1 | State Selection | Identify the best state to launch outreach, ensuring demographic and spending alignment |
| ✅ Phase 2 | ZIP-to-County Aggregation | Reveal top counties in target state using population and purchase trends |
| ✅ Phase 3 | Trade Area Definition | Focus on neighborhoods with highest target group concentration |
| ✅ Phase 4 | Retail Partner & Buyer Estimation | Select best store hub to distribute kits and forecast buyer volume |
| ✅ Phase 5 | Lifestyle Segmentation | Understand local attitudes, values, and income to tailor outreach |
| ✅ Phase 6 | Scalability Modeling | Identify lookalike trade areas for regional expansion |

---

## 📍 Phase 1: State Selection

We used Alteryx + Esri 2024 data to evaluate where Hispanic women aged 15–44 are most concentrated, and where skincare spend is meaningful.

### 📸 Key Screenshots
- 🧮 [Total Hispanic Female Count Formula](./assets/alteryx_formula_sum_hispanic_females_15_44.png)
- 📊 [Percent of Population Formula](./assets/alteryx_formula_percent_hispanic_females_15_44.png)
- 📈 [State-Level Output Table](./assets/alteryx_output_state_selection_hispanic_spend.png)
- 🔎 [Hispanic Age Group Selection in Esri](./assets/esri_data_browser_hispanic_age_selection.png)
- 💄 [Skincare Spend Variable in Esri](./assets/esri_data_browser_cosmetics_spending_variable.png)

---

## 📍 Phase 2: ZIP-to-County Aggregation

We aggregated ZIP-level data into counties to locate high-impact areas within New Mexico.

### 📸 Key Screenshots
- 🔧 [ZIP-to-County Enrichment Workflow](./assets/alteryx_workflow_zipcode_enrichment_and_county_join.png)
- 📊 [Summarize by County](./assets/alteryx_summarize_groupby_county_metrics.png)
- 📍 [Enriched ZIP-Level Table](./assets/zip_level_enrichment_table.png)
- 📈 [Sort Counties by % in Target Group](./assets/alteryx_sort_county_by_usergroup_percentage.png)
- 🧮 [Sort by Raw Count of Target Group](./assets/alteryx_sort_counties_by_total_target_group.png)

---

## 📍 Phase 3: Trade Area Definition

Focused on block groups in Bernalillo County with ≥280 Hispanic women aged 15–44.

### 📸 Key Screenshots
- 🧮 [Threshold Calculation from Summary Stats](./assets/alteryx_profile_statistics_hisp1545_threshold.png)
- 📍 [Alteryx Filtered Block Groups Workflow](./assets/alteryx_map_and_workflow_filtered_trade_areas.png)
- 📌 [Target ZIP 87121 Map](./assets/arcgis_trade_area_map_target_zip_87121.png)
- 🗺 [Map Legend View](./assets/arcgis_trade_area_map_legend.png)

---

## 📍 Phase 4: Retail Partner & Buyer Estimation

Used fixed-radius trade areas and spending data to find best store hub (Sunficent LLC).

### 📸 Key Screenshots
- 🛠️ [Retail Address Workflow in Alteryx](./assets/alteryx_workflow_beauty_retailer_addresses_87121.png)
- 🗺 [Overlapping Trade Area Cleanup](./assets/arcgis_trade_area_map_remove_overlap_87121.png)
- 📊 [Store Comparison Table](./assets/alteryx_trade_area_comparison_87121.png)
- 🧮 [Buyer Estimation Formula](./assets/alteryx_estimate_total_buyers_sunficent.png)
- 🎯 [Target Group Buyer Estimate](./assets/alteryx_estimate_target_group_reach_sunficent.png)

---

## 📍 Phase 5: Lifestyle Segmentation

We used Esri Tapestry segments to understand behavioral traits in the chosen trade area.

### 📸 Key Screenshots
- 🗺 [Segment Map: Sunficent Trade Area](./assets/arcgis_tapestry_segments_trade_area_sunficent.png)
- 🛠️ [Workflow: Segment Enrichment in Alteryx](./assets/alteryx_workflow_enriched_trade_area_segmentation.png)
- 📊 [Tapestry Household Counts](./assets/alteryx_tapestry_segmentation_output_sunficent.png)
- 📈 [Tapestry Segment % Breakdown](./assets/alteryx_tapestry_segmentation_percentages_sunficent.png)
- 🧬 [Segment 7A Summary](./assets/tapestry_7A_summary_traits.png)
- 🧮 [7A Demographics](./assets/tapestry_7A_demographics_spending.png)
- 🧠 [7A Market Indices](./assets/tapestry_7A_market_profile_indices.png)

---

## 📍 Phase 6: Scalability Modeling

Scraped nearby skincare retailers and evaluated trade areas for similar 7A alignment.

### 📸 Key Screenshots
- 🌐 [ParseHub Scrape – Yellow Pages](./assets/parsehub_scrape_yellowpages_cosmetics_87120.png)
- 🛠️ [Workflow: Clean Scraped Addresses](./assets/alteryx_cleaning_scraped_addresses_87120.png)
- 📊 [Compare New Trade Areas by 7A Households](./assets/alteryx_trade_area_comparison_7A_expansion.png)

  ---

## 💼 Business Impact & Social Relevance

This project demonstrates how **micromarketing + spatial analytics** can unlock both business value and community wellness.

### 🔹 For Business:
- 🎯 **Hyper-targeted outreach** to ZIPs and counties with verified demand
- 📈 **Higher ROI** through value-based campaigns in high-conversion neighborhoods
- 🧭 **Data-backed expansion** using psychographics and geospatial analysis
- 🤝 **Retail partnership strategy** to lower costs and build local trust

### 🔹 For Communities:
- ❤️ **Culturally relevant skincare access** for underserved populations
- 💡 **Health equity + self-confidence** through informed personal care
- 🌍 **Scalable outreach model** that aligns profit with purpose

> This work bridges data science, retail strategy, and human impact — proving that inclusive marketing is not only ethical, but also strategic.

---

## 👤 Author

**Pratiksha Gund**  
📍 Data Analyst | Micromarketing Researcher  
🔗 [LinkedIn](https://www.linkedin.com/in/pratiksha-gund/) | 🌐 [Portfolio]() | ✉️ [pratikshagund10@gmail.com](mailto:pratikshagund10@gmail.com)

---

## 🏷 Tags

#Micromarketing #GIS #RetailAnalytics #Alteryx #ArcGIS #ConsumerInsights  
#InclusiveSkincare #BehavioralTargeting #DataForGood #TradeAreaModeling #TapestrySegmentation

