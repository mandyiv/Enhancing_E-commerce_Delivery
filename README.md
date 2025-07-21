# Enhancing E-commerce Delivery Efficiency through Advanced Analytics and Machine Learning

## Project Overview  
This project addresses the critical challenge of delivery delays in the competitive e-commerce logistics landscape. Leveraging a comprehensive dataset of historical deliveries, this initiative aims to identify and prevent delays, optimise internal warehouse operations (packaging and batching), and establish a robust routing framework to improve Service Level Agreement (SLA) adherence and customer satisfaction.

---

## Goal  
To identify and prevent delivery delays, optimise packaging and batching logic, and build a routing framework that improves SLA adherence and customer satisfaction.

---

## Solution Approach
A multi-faceted approach was adopted, comprising four key analytical pillars:

1. **Exploratory Data Analysis (EDA):** Uncovering operational bottlenecks and key data patterns.

2. **Order Clustering:** Optimising packaging and batching logic by grouping orders with similar operational characteristics.

3. **Predictive Modelling:** Developing a machine learning model to score future deliveries by their risk of delay, enabling proactive intervention.

4. **Routing Logic & Courier Rules:** Deriving actionable rules to optimise last-mile delivery performance based on product attributes and courier capabilities.

---

## Key Insights

- **Significant Delay Rate:** Approximately 40.3% of deliveries experienced delays, highlighting a substantial challenge.

- **Weight as a Critical Factor:** 'Medium' weight items show near-perfect on-time delivery (99.9%), while 'Heavy' items consistently exhibit the worst performance (56.8% delay rate) across all couriers, indicating a systemic operational challenge.

- **Discount-Driven Prioritisation:** Orders with discounts over 10% achieve a striking 100% on-time delivery rate, suggesting a strong, likely intentional, operational prioritisation for promotional campaigns.

- **Suboptimal Courier & Mode Matching:**

      - High-priority items are not consistently routed via faster modes; surprisingly, 'Road' and 'Ship' modes often outperform 'Flight' for these.
      
      - `Courier_1` consistently underperforms, especially for high-priority and heavy items. `Courier_4` and `Courier_5` show superior performance for high-importance items.

- **Customer Care Calls as Early Warning:** An increase in customer care calls strongly correlates with a decrease in on-time delivery rates.

- **Operational Clusters:** Orders naturally group into three distinct clusters based on weight, discount, cost, and importance, enabling tailored batching and packaging strategies.

- **Predictive Power:** A CatBoost model achieved a high recall of 0.95 for identifying late deliveries, demonstrating strong potential for proactive delay mitigation. `Discount_offered` and `Weight_in_gms` were the most influential features in predicting delays.

---

##  Final Recommendations

- **Re-engineer heavy shipment processes**: Focus on packaging, handling, and last-mile delivery  
- **Dynamic courier assignment**: Match couriers to product weight and priority  
- **Scale discount-based prioritisation**: Extend current high-discount success logic to all urgent orders  
- **Integrate predictive delay alerts**: Use model insights for proactive operational intervention  
- **Tailor batching by cluster**: Implement specific workflows per identified operational group  

---

## Technologies Used

- Python (Pandas, Matplotlib, Seaborn, Scikit-learn) 
- Machine Learning (CatBoost, XGBoost, LightGBM, ExtraTrees, RandomForest, Logistic Regression)
- Jupyter Notebook  

---

## How to Use

1. **Clone this repository**  
```bash
git clone [repository-url]
```
2. **Navigate to the project directory** 
``` bash
cd [project-directory]
```
3. **Install dependencies**
``` bash
pip install -r requirements.txt
```
4. **Load the dataset**
Place your Enhanced_Ecommerce_Shipping_Data.csv in the root folder
(Or update the path in the notebook.)

5. **Run notebooks**
Explore the project through EDA, Clustering, and Modelling notebooks.

---

## **Future Work & Next Steps**  
- Pilot A/B testing of routing and batching strategies

- Real-time model integration with operational dashboards

- Deep-dive analysis into Flight mode underperformance

- Extend model with external data (e.g., traffic, weather)

- Develop an automated routing engine

- Implement continuous feedback & model retraining

---

## **Author & Contact**  
**Amanda Osaikhuwuomwan**  
[Email Me](mailto:osaiamanda@gmail.com)  
[Connect on LinkedIn](https://www.linkedin.com/in/amandaosai/)  
