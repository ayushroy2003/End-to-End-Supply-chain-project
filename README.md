# 🌟 What is Supply Chain Delivery Performance Analysis & Predictive Insights?

**Supply Chain Delivery Performance Analysis & Predictive Insights** is a data analysis project that studies why e-commerce orders are delivered late and how those delays affect business profitability.

The project analyzes **172,765 orders** from January 2015 through January 2018. It combines delivery performance analysis, profitability analysis, bottleneck detection, root-cause analysis, time-based analysis, and machine learning.

Think of it like a **health check for an e-commerce delivery system**. It identifies where delivery problems are happening, measures their business impact, finds the most important problem areas, and predicts which orders may be at risk of late delivery.

The main finding is that **54.71% of analyzed orders were delivered late**, with **$2.1M in profit at risk on delayed orders**.

---

# 🚀 What it Does (Features)

- 📊 **Measures delivery performance**
  - Analyzes total orders, late deliveries, and on-time deliveries.
  - Calculates the overall late-delivery rate.

- 💰 **Measures financial impact**
  - Analyzes the relationship between delivery delays and order profitability.
  - Estimates the profit associated with delayed orders.
  - Helps connect operational problems with business impact.

- 📈 **Analyzes profitability**
  - Classifies orders into:
    - Profit
    - Loss
    - Breakeven
  - Examines profit across different delay levels.

- 🚨 **Identifies operational bottlenecks**
  - Compares delivery delays across:
    - Region
    - Customer Segment
    - Shipping Mode
    - Order Status
    - Payment Type
    - Department
  - Identifies **shipping mode as the strongest operational differentiator**.

- 🔍 **Performs root-cause analysis**
  - Investigates the region with the highest reported delay rate.
  - Identifies important delay drivers related to shipping mode, payment/order status, payment type, and product departments.

- 🕐 **Analyzes time-based patterns**
  - Studies delivery delays by:
    - Month
    - Day of Week
    - Hour of Day
  - Helps identify periods where capacity and processing may need additional attention.

- 🤖 **Predicts late deliveries**
  - Uses a **Random Forest machine-learning model** to predict whether an order is likely to be delivered late.
  - Uses **SMOTE**, a technique used to balance uneven groups of data.
  - The reported model achieved **74% accuracy**.

- 🎯 **Provides business recommendations**
  - Recommends actions based on the findings.
  - Prioritizes improvements according to business importance.

---

# 🛠️ How to Use It (Step-by-Step)

This project is built using **Python and Jupyter Notebook**.

Jupyter Notebook is an interactive environment where you can run Python analysis one section at a time.

### Step 1: Install Python

Download and install Python from the official website:

https://www.python.org/

After installation, open **Command Prompt** on Windows or **Terminal** on macOS/Linux.

Check whether Python is installed:

```bash
python --version
