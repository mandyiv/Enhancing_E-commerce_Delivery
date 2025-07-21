# Enhancing E-commerce Delivery Efficiency through Advanced Analytics and Machine Learning

## Project Overview  
This project addresses the critical challenge of **delivery delays** in the fast-paced e-commerce logistics space. Using a rich dataset of 10,999 historical deliveries, we aimed to identify and prevent delays, improve warehouse batching and packaging logic, and develop a robust routing framework to improve **SLA adherence** and **customer satisfaction**.

---

## Goal  
- Predict and prevent delivery delays  
- Optimise packaging and batching processes  
- Design a courier assignment framework based on operational performance  

---

## Solution Approach

1. **Exploratory Data Analysis (EDA)**  
   - Uncovered key patterns, bottlenecks, and data quality issues

2. **Order Clustering**  
   - Segmented deliveries into operational clusters for optimised batching and packaging

3. **Predictive Modeling**  
   - Built a machine learning model (CatBoost) with **95% recall** to flag potential delays

4. **Routing Logic & Courier Rules**  
   - Developed dynamic rules for last-mile delivery optimisation based on weight and product importance

---

## Key Insights

- **40.3% of deliveries** experienced delays — a major performance gap  
- **Medium-weight items (2001–4000g)** had **99.9% on-time rate** → operational sweet spot  
- **Heavy items** had the **highest delay rate (56.8%)**, regardless of courier  
- **Orders with >10% discounts** had **100% on-time delivery**, showing promo-driven prioritization  
- **Courier_1** consistently underperformed for **high-priority and heavy shipments**  
- **Courier_4 & 5** demonstrated superior, consistent performance  
- **Customer care calls** were early indicators of delivery risk  
- Operational clustering revealed 3 order types ideal for tailored batching workflows  
- **Top delay predictors:** `Discount_offered`, `Weight_in_gms`

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
