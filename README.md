

# 🛒 Market Basket Optimization using Apriori

This project demonstrates how to uncover **frequent itemsets** and generate **association rules** using the **Apriori algorithm** for Market Basket Analysis. It aims to identify product combinations that frequently co-occur in transactions, which can be used for improving sales strategies.

---

## 📌 Problem Statement

Given a dataset of customer transactions, the goal is to discover **frequent itemsets** and **association rules** to better understand customer buying habits.

---

## 💡 What is Market Basket Analysis?

Market Basket Analysis is a data mining technique used by retailers to increase sales by better understanding customer purchase patterns. For example, if a customer buys bread and butter, they are likely to buy jam.

---

## 📊 Dataset

* Dataset: A transactional dataset (e.g., `Market_Basket_Optimisation.csv`)
* Each row represents a transaction (items purchased together)
* Format: Items are stored as strings, separated by commas in each row

Example:

```
Milk, Bread, Butter
Bread, Eggs
Milk, Bread, Eggs, Cheese
```

---

## 🧠 Algorithm Used

* **Apriori Algorithm** from the `apyori` library
* Generates frequent itemsets based on **support**
* Derives association rules using **confidence**, **lift**
---

## 🔍 Steps Involved

1. **Data Preprocessing**

   * Load and clean transaction data
   * Convert data into a list of transactions

2. **Frequent Itemset Mining**

   * Use `Apriori` to extract frequent itemsets based on minimum support

3. **Association Rule Mining**

   * Apply `association_rules` to generate rules from frequent itemsets
   * Filter by metrics: confidence, lift

---

## 🛠️ Tools & Libraries

* Python
* Pandas, NumPy
* Apyori
* Matplotlib, Seaborn

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/market-basket-optimisation-apriori.git
   cd market-basket-optimisation-apriori
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:

   * Open `market_basket_apriori.ipynb` in Jupyter Notebook or Google Colab
   * Execute the cells step-by-step

---

## 📈 Sample Results

* **Top Frequent Itemsets**:

  * Bread & Butter
  * Milk & Bread
  * Eggs & Cheese

* **Sample Association Rule**:

  ```
  IF {Bread, Butter} THEN {Milk}
  Confidence: 0.74
  Lift: 1.5
  ```

