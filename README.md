# Inclusive Skincare Access: A Geo-Demographic Micromarketing Project

This project uses data science, spatial analytics, and micromarketing to identify and prioritize outreach opportunities for **inclusive skincare access** among **Hispanic women aged 15–44**—a fast-growing, underrepresented demographic in the wellness space.

Each phase is grounded in real data and business logic, designed to be scalable, replicable, and community-driven. This project not only empowers equitable access to wellness but also models how brands can achieve **targeted growth** while driving **social impact**.

---

## 🧠 Why This Matters: Business & Community Value

Micromarketing allows businesses to move beyond generic campaigns and instead connect with **high-need, high-opportunity micro-audiences**. This project shows how skincare and wellness brands can:

- Identify **where real demand exists**, using demographic density and spend potential
- Serve **culturally aligned messaging** to those most likely to respond
- Launch **cost-efficient outreach** in geographies that maximize ROI
- Enable **social good** by making health and beauty more accessible

The outcome? Smarter campaigns, greater consumer trust, and scalable growth rooted in inclusion.

---

## 🗂️ Project Workflow Overview

| Phase | Description | Why It Matters |
|-------|-------------|----------------|
| Phase 1 | **State Selection** | Identify the best state to launch outreach, ensuring demographic and spending alignment |
| Phase 2 | **ZIP-to-County Aggregation** | Reveal top counties in target state using population and purchase trends |
| Phase 3 | **Trade Area Definition** | Focus on neighborhoods with highest target group concentration |
| Phase 4 | **Retail Partner & Buyer Estimation** | Select best store hub to distribute kits and forecast buyer volume |
| Phase 5 | **Lifestyle Segmentation** | Understand local attitudes, values, and income to tailor outreach |
| Phase 6 | **Scalability Modeling** | Identify lookalike trade areas for regional expansion |

---

## 🔧 Tools & Data Sources

- **Alteryx Designer** – ETL, formula logic, summarization, spatial joins
- **ArcGIS Pro** – Mapping, segment layers, buffer zones
- **Esri Demographics (2024)** – Age, sex, race, consumer spend, lifestyle segments
- **Census Data** – County and ZIP code boundaries, FIPS, block groups
- **ParseHub** – Scraping retail data from Yellow Pages

---

## 📍 Phase Highlights

### Phase 1: State Selection  
Use demographic filters to shortlist states with both **high Hispanic female density (15–44)** and **strong skincare spending**.

> 🧠 Why: Sets up strategic geographic focus before going local.

---

### Phase 2: ZIP ➡ County Aggregation  
Aggregate enriched ZIP data to county level to see **where outreach can scale** across ZIP clusters.

> 🧠 Why: Identifies counties with high outreach efficiency (user density × ZIPs × spend)

---

### Phase 3: Trade Area Identification  
Create filters based on statistical thresholds (e.g., mean + 1 SD) to define **high-opportunity block groups**.

> 🧠 Why: Moves targeting from broad county to hyperlocal level.

---

### Phase 4: Retail Partner Evaluation  
Map 1-mile radius trade areas around beauty stores. Select based on projected **user count, spend**, and **market diversity**.

> 🧠 Why: Ensures distribution points are viable and aligned with community needs.

---

### Phase 5: Lifestyle Segmentation  
Use Esri Tapestry segments to understand **household behavior**, then match future trade areas to top segments (e.g., 7A: Up & Coming Families).

> 🧠 Why: Informs messaging, outreach channels, and local preferences.

---

### Phase 6: Scalability  
Scrape nearby locations, enrich with same logic, and rank by segment 7A household count to identify **next trade area**.

> 🧠 Why: Makes project repeatable and ready to expand to similar areas.

---

## 🗺️ Screenshots & Workflows

> 📁 All visuals are available in the `/assets` folder to demonstrate each step visually.

- Alteryx calculations
- Map legends
- Trade area overlays
- Segment breakdowns
- Retail partner comparisons

---

## 📣 Final Thoughts

This project models how micromarketing + spatial analysis can power **inclusive wellness outreach** using real demographic and consumer behavior data.

Every step—from macro targeting to lifestyle analysis—is grounded in market logic, ensuring brands not only grow but **grow responsibly**.

The final phase will explore **campaign modeling and impact estimation** for each selected area.

---

## 👩‍💼 Author

**Pratiksha Gund**  
📍 Data Analyst | Micromarketing Researcher  
🔗 [LinkedIn](https://www.linkedin.com/in/pratiksha-gund/) | 🌐 [Portfolio] | ✉️ [pratikshagund10@gmail.com](mailto:pratikshagund10@gmail.com)

---

## 🏷 Tags

#Micromarketing #GIS #RetailAnalytics #Alteryx #ArcGIS #DataForGood  
#ConsumerInsights #InclusiveSkincare #BehavioralTargeting #TradeAreaModeling
