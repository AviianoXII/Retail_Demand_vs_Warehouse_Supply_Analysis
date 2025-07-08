# Retail Demand vs Warehouse Supply Analysis


This project investigates the disparity between retail demand and warehouse supply across multiple suppliers and product categories in the beverage industry. By analyzing over 300,000 transactional records, the objective is to identify gaps, inefficiencies, and opportunities for operational improvements in supply chain performance.
The interactive Power BI dashboard can be found [here](https://app.powerbi.com/links/yE_LbM5bUR?ctid=d73c3455-2ff8-4748-95c8-611e0bf264e1&pbi_source=linkShare), and Kaggle notebook [here](https://www.kaggle.com/code/xiiaviiano/retail-demand-vs-warehouse-supply).

![](https://github.com/AviianoXII/Retail_Demand_vs_Warehouse_Supply_Analysis/blob/main/IMG_4206.png)

## Research Questions


- How well does warehouse supply meet retail demand across different suppliers and time periods?
- What are the top contributors to supply-demand imbalance?
- Which items show the greatest sales gaps or overstocking/understocking 

---

## 📌 Important Metrics & Dimensions

### Metrics (from the dataset)
- **`retail_sales`**: Quantity sold at retail level

  
- **`warehouse_sales`**: Quantity supplied from warehouse

  
- **`sales_gap`**: Difference between warehouse and retail sales

  
- **`gap_ratio`**: Ratio of retail demand to warehouse supply


### Dimensions
- **`supplier`**: Identifies the source of products

  
- **`item_description`**: Describes the specific product

  
- **`item_code`**: Unique identifier for each product

  
- **`year`**: Year of transaction

  
- **`month`**: Month of transaction

---

## Summary of Insights

- 🟣 **Imbalance in Supply Chain:** The average `gap_ratio` suggests that for every unit sold at retail, nearly double was available at the warehouse, highlighting overstocking.
- 🟢 **Overstocked Items:** Approximately 176,000 items had higher warehouse sales than retail sales, suggesting inefficient demand forecasting or oversupply.
- 🔴 **Understocked Items:** Over 128,000 items were understocked, pointing to missed sales opportunities and poor replenishment planning.
- 🟡 **Top Gaps by Supplier & Item:** Suppliers such as CORONA and HENEKEN (truncated names from dashboard) consistently appeared among the top contributors to sales gaps.
- 🔵 **Temporal Trends:** Retail demand remains relatively consistent month-to-month, while warehouse supply varies more significantly, contributing to the sales gap volatility.

---

## ✅ Recommendations

### 1. **Dynamic Replenishment Modeling**
- **Finding**: A significant portion of items (~176,000) were overstocked, while over 128,000 were understocked, indicating frequent mismatches between warehouse supply and retail demand.  

- **Action**: Develop predictive restocking models using item-level `gap_ratio` and `sales_gap` trends to forecast demand more accurately.  

- **Why This Matters**: Aligning warehouse supply with actual retail demand minimizes inventory holding costs and prevents lost sales due to understocking.  


---

### 2. Supplier Performance Benchmarking
- **Finding**: Certain suppliers, like **CORONA** and **HENEKEN**, frequently appear among the top contributors to sales gaps.  

- **Action**: Rank suppliers based on average `gap_ratio` and total contribution to `sales_gap` to identify those with chronic mismatches.  

- **Why This Matters**: Holding suppliers accountable improves upstream performance and fosters more reliable fulfillment planning.  

---

### 3. Item Prioritization
- **Finding**: Some products consistently experience large understocking gaps, despite steady retail demand.  

- **Action**: Prioritize inventory planning efforts on the top 10 understocked items by `sales_gap`.  

- **Why This Matters**: Focusing on high-impact items delivers better ROI, as even small adjustments can significantly reduce lost sales and improve customer satisfaction.  

---

## 📫 Author

**Name:** Karlon Mc Lean  
[LinkedIn](https://www.linkedin.com/in/karlon-mc-lean-b613101b3/)
