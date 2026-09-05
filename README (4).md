# 🌟 What is Supply Chain Delivery Performance Analysis & Predictive Insights?

**Supply Chain Delivery Performance Analysis & Predictive Insights** is a data analysis project that studies why e-commerce orders are delivered late and how those delays affect business profitability. It analyzes **172,765 orders** from January 2015 through January 2018 and combines business analysis, charts, bottleneck analysis, root-cause analysis, time-based analysis, and a machine-learning model.

Think of it like a **health check for an e-commerce delivery system**: the project looks at where delivery problems happen, measures how serious they are, identifies the areas that need attention first, and uses a predictive model to flag orders that may be late.

The main reported finding is that **54.71% of analyzed orders were delivered late**, while the reported profit at risk on delayed orders was **$2.1M**.

---

# 🚀 What it Does (Features)

- **Measures overall delivery performance**
  - Calculates total orders, late deliveries, late-delivery rate, and on-time delivery rate.
  - Establishes a clear performance baseline for the business.

- **Measures the financial impact of delays**
  - Compares delivery delays with order-level profit.
  - Shows how much profit is associated with delayed orders.
  - Helps connect an operational problem with a business outcome.

- **Analyzes profitability**
  - Classifies orders as **Profit, Loss, or Breakeven**.
  - Shows the percentage of orders in each profitability group.
  - Examines profit and order volume across different delay levels.

- **Finds operational bottlenecks**
  - Compares delay rates across:
    - Region
    - Customer segment
    - Shipping mode
    - Order status
    - Payment type
    - Department
  - The report identifies **shipping mode as the strongest differentiating operational area**.

- **Performs root-cause analysis**
  - Looks more deeply at the region with the highest reported delay rate.
  - Highlights factors such as shipping mode, payment/order status, payment type, and product departments.

- **Finds time-based patterns**
  - Examines delays by:
    - Month
    - Day of the week
    - Hour of the day
  - Helps identify periods that may need additional capacity or process review.

- **Predicts delivery risk**
  - Uses a **Random Forest** machine-learning model to predict whether an order is likely to be delivered late.
  - Uses **SMOTE (a technique for balancing uneven groups of data)** before model training.
  - The reported test results show **74% accuracy**, with **0.78 precision for late-order predictions** and **0.75 recall for actual late orders**.

- **Turns analysis into business recommendations**
  - Prioritizes actions such as reviewing First Class and Second Class shipping performance, deploying predictive alerts, resolving payment-processing bottlenecks, and planning for seasonal demand.

---

# 🛠️ How to Use It (Step-by-Step)

This project is designed to be run as a **Jupyter Notebook**, which is an interactive document where you can run Python analysis one section at a time.

### 1. Install Python

If Python is not already installed on your computer, install a recent version of Python.

You can use the official Python website:

https://www.python.org/

### 2. Install Jupyter Notebook

Open a terminal or Command Prompt and run:

```bash
pip install notebook
```

If the `pip` command does not work, try:

```bash
python -m pip install notebook
```

### 3. Install the project libraries

The notebook uses the following Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

These libraries are used for working with data, creating charts, and building the predictive model.

### 4. Put the required files in the same folder

Place these files together in one project folder:

```text
Supply-Chain-Project/
│
├── supply.ipynb
├── DataCoSupplyChainDataset.csv
└── README.md
```

**Important:** the notebook reads the dataset using the filename:

```text
DataCoSupplyChainDataset.csv
```

So the CSV should have that exact filename and should be in the same folder as the notebook.

### 5. Open the project

Open Command Prompt or Terminal.

Go to the folder containing the project. For example:

```bash
cd path/to/Supply-Chain-Project
```

Then start Jupyter Notebook:

```bash
jupyter notebook
```

A browser window should open with the Jupyter Notebook interface.

### 6. Open `supply.ipynb`

Click:

**`supply.ipynb`**

This opens the main analysis notebook.

### 7. Run the notebook from the beginning

Run the cells from top to bottom.

In Jupyter Notebook, you can usually run a cell by clicking the **Run** button.

Running the notebook in order is recommended because later sections use calculations created in earlier sections.

### 8. Review the results

The notebook produces analysis covering:

1. Business problem and desired outcome
2. Data overview and cleaning
3. Exploratory data analysis
4. Delivery-delay calculations
5. Profitability analysis
6. Bottleneck detection
7. Root-cause analysis
8. Time-based delay analysis
9. Random Forest prediction model
10. Model performance results

The accompanying report summarizes these findings in a business-friendly format.

### 9. Read the report for the business conclusions

The project report is useful if you want to understand the results without reading the Python code.

The report highlights the major findings, charts, model results, recommendations, and target improvements.

---

# 📂 What's Inside?

A simple project structure looks like this:

```text
Supply-Chain-Project/
│
├── supply.ipynb
├── DataCoSupplyChainDataset.csv
└── README.md
```

### `supply.ipynb`

This is the **main analysis file**.

It contains the Python work used to:

- Clean and prepare the data
- Calculate delivery delays
- Measure business KPIs (Key Performance Indicators, meaning important business measurements)
- Analyze profitability
- Find delivery bottlenecks
- Investigate possible root causes
- Study time-based delay patterns
- Train and evaluate the Random Forest model

### `DataCoSupplyChainDataset.csv`

This is the **data file** used by the notebook.

It contains the order-level supply-chain information needed for the analysis.

The notebook loads this file directly, so it must be available in the expected project folder.

### `README.md`

This file explains the project in simple language.

It is intended for:

- Recruiters
- Interviewers
- Clients
- Business stakeholders
- Beginners who want to understand the project

### Project Report

The project report presents the analysis as a business report. It includes the performance dashboard, profitability analysis, bottleneck detection, root-cause analysis, time-based patterns, machine-learning results, recommendations, and conclusion.

---

# ❓ Frequently Asked Questions

### 1. Do I need to know Python to understand the project?

**No.**

The report is written to explain the business findings without requiring programming knowledge.

However, if you want to run or modify the notebook yourself, basic Python and Jupyter Notebook knowledge will be helpful.

### 2. What if the notebook says it cannot find `DataCoSupplyChainDataset.csv`?

Make sure the CSV file is in the **same folder as `supply.ipynb`** and that its filename is exactly:

```text
DataCoSupplyChainDataset.csv
```

The notebook specifically loads the dataset using this filename.

### 3. What if I only want to see the results and not run the code?

You can read the project report without running the notebook.

The report already presents the main business findings, including the reported **54.71% late-delivery rate**, **$2.1M profit at risk on delayed orders**, and **74% Random Forest accuracy**.

### 4. Do I need to pay for anything?

The project itself is based on Python and commonly used Python data-analysis libraries. The notebook does not require a paid software platform to run.

You do need the project dataset (`DataCoSupplyChainDataset.csv`) to reproduce the analysis.

---

## 📌 Key Results at a Glance

| Metric | Reported Result |
|---|---:|
| Orders analyzed | 172,765 |
| Late deliveries | 94,523 |
| Late delivery rate | 54.71% |
| On-time delivery rate | 45.29% |
| Total profit from profitable orders | $7.5M |
| Profit at risk on delayed orders | $2.1M |
| 90th-percentile delay | 3 days |
| Random Forest accuracy | 74% |
| Precision for late orders | 0.78 |
| Recall for late orders | 0.75 |

## 🎯 Main Business Goal

The analysis provides a data-driven basis for improving delivery reliability, protecting profitable orders, and reducing the financial impact of late deliveries.

The report's target states include reducing the late-delivery rate to **below 30% within 12 months**, improving First Class and Second Class on-time performance, increasing predictive-model accuracy, reducing loss-making orders, and reducing profit at risk.
