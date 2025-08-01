# DoorDashNewVerticals

<!-- Header Image -->
<p align="center">
  <img src=".\img\dashmart_logo.png" alt="Project Header" style="width:40%; max-width:200px;">
</p>

# 📁 Executive Summary

**TLDR**: Dashmart makes 70% of the Cincinnati market, with highest in-stock rate (99.66%), lowest substitution rate (0.11%) & fastest D2R (2.91 minutes). The business is driven by early morning weekend orders occurring between 12am - 4am, Fri-Sun. Opportunity lies in increasing produce/diary market penetration & order packing efficiency.

**Produce/Dairy**
Dashmart does well in convenience items (snacks/drinks/pantry/candy) but poorly in produce/dairy compared to other grocers. Based on seasonality + types of products purchased consumers are likely utilizing Dashmart for ‘fun food’ versus their regular grocery shopping. 

Should Dashmart want to cannibalize regular grocery shopping from competitors, we will need to:
- Validate produce/dairy offerings & price match competitors
- Offer targeted ads to users who primarily use other grocers for produce/diary

**Packing Efficiency (Lates)**
Dashmart has the fastest D2R & similar CLAT to other grocers but one of the highest rates of lates. While CLAT is the primary indicator if an order will be late this is followed by D2R. Since CLAT is the same, D2R is lower, we would expect lates to be on the lower end of the market. 

**We can infer there may be issues with packing orders timely so drivers are waiting at Dashmart driving lates.** This could also explain why drivers are hesitant to accept Dashmart orders even though they are close by the facility

# 📖 Table of Contents

- [Data Prep](#data-prep)
- [Analysis](#analysis)
- [Tableau](#tableau)

  
# <h1 id="data-prep">📊 Data Prep</h1>

### Google BigQuery (GBQ)
Utilized [GBQ]([https://example.com](https://console.cloud.google.com/bigquery?hl=en&inv=1&invt=Ab2rzQ&project=zeta-matrix-337222&ws=!1m0)) as data warehouse & primary data prep tool

**Keywords** used: *SELECT/FROM/GROUPBY*
<br>
**Functions** used: *IF/SUM/MAX/COUNT/EXTRACT*

#### Wrangling
-  Input from gsheet (had issues moving to GBQ directly from CSV due to special characters in item names)
-  Normalize column names
-  Convert time from UTC to EST
-  Remove duplicates (1 delivery/item mapped twice due to 2 different prices being listed

# <h1 id="analysis">📈 Analysis</h1>

Full Analysis can be found [View the Report](./Output/DD%20Case%20Study.pdf)

# <h1 id="tableau">🖥️ Tableau</h1>

Tableau published sheets can be viewed [here](https://public.tableau.com/app/profile/candice.filar/viz/DashmartNewVerticals/StoreoverTime)
