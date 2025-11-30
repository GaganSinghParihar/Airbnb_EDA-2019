 Airbnb NYC 2019 EDA project.
It includes:

✔ Project Overview
✔ Business Context
✔ Dataset Description
✔ Folder Structure
✔ Installation
✔ How to Run
✔ EDA Summary + Sample Visuals
✔ Final Conclusion
✔ Future Scope

This is **copy-paste ready** into your GitHub repository.

---

# 🏡 **Airbnb NYC 2019 — Exploratory Data Analysis (EDA)**

A complete industry-level EDA project analyzing **48,834 Airbnb listings** across New York City to uncover pricing behavior, neighbourhood trends, host patterns, and demand signals.

---

# 📌 **1. Project Overview**

Airbnb has transformed the global hospitality industry, enabling individuals to host travelers and provide personalized accommodation. With millions of listings worldwide, data plays a crucial role in:

* Understanding customer and host behavior
* Monitoring supply-demand patterns
* Improving pricing strategies
* Enhancing platform performance

This project performs **end-to-end Exploratory Data Analysis (EDA)** on **Airbnb NYC 2019 dataset**.
It follows a realistic workflow used in the data industry, including:

✔ Data loading
✔ Data cleaning
✔ Handling missing values
✔ Outlier removal
✔ Feature exploration
✔ Visualization
✔ Statistical insights
✔ Business recommendations

---

# 💼 **2. Business Context**

The goal is to analyze NYC Airbnb listings to answer:

* **What drives pricing in New York City?**
* **Which neighbourhoods are the most expensive?**
* **Which room types generate the most revenue?**
* **How do availability and reviews affect listing performance?**
* **What insights can help hosts optimize their listings?**

This analysis helps hosts, investors, and Airbnb understand market behavior and demand patterns.

---

# 📂 **3. Dataset Description**

The dataset contains Airbnb listing information from NYC across 5 boroughs:

| Column Name                    | Description                                |
| ------------------------------ | ------------------------------------------ |
| id                             | Listing ID                                 |
| name                           | Listing title                              |
| host_id                        | Unique Host ID                             |
| host_name                      | Name of the host                           |
| neighbourhood_group            | Manhattan, Brooklyn, etc.                  |
| neighbourhood                  | Specific locality                          |
| latitude                       | Latitude coordinate                        |
| longitude                      | Longitude coordinate                       |
| room_type                      | Entire home/apt, Private room, Shared room |
| price                          | Price per night                            |
| minimum_nights                 | Minimum nights required                    |
| number_of_reviews              | Total reviews                              |
| last_review                    | Date of last review                        |
| reviews_per_month              | Review frequency                           |
| calculated_host_listings_count | Number of listings by host                 |
| availability_365               | Days available per year                    |

Dataset Size: **48,834 rows × 16 columns**
Mix of numeric and categorical variables.

---

# 🏗 **4. Project Structure**

```
Airbnb_EDA/
│
├── data/
│   ├── airbnb_nyc_2019.csv
│   └── airbnb_cleaned.csv
│
├── notebooks/
│   ├── 01_data_loading.ipynb
│   ├── 02_data_cleaning.ipynb
│   └── 03_EDA.ipynb
│
├── src/
│   ├── cleaning.py
│   ├── visualizations.py
│   └── utils.py
│
├── images/
│   └── plots/
│
└── README.md
```

This structure follows **industry best practices** for scalable analytics projects.

---

# ⚙️ **5. Installation & Setup**

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/Airbnb_EDA-2019.git
cd Airbnb_EDA-2019
```

### 2️⃣ Create virtual environment

```bash
python -m venv venv
source venv/bin/activate     # Mac/Linux
venv\Scripts\activate        # Windows
```

### 3️⃣ Install required libraries

```bash
pip install -r requirements.txt
```

---

# ▶️ **6. How to Run the Project**

### **Run Cleaning Script**

```bash
python src/cleaning.py
```

### **Run EDA Notebook**

Open Jupyter Notebook and run:

```
notebooks/03_EDA.ipynb
```

This will generate plots and analysis stored in `images/plots/`.

---

# 📊 **7. Exploratory Data Analysis (Summary)**

Below is a summary of the major visualizations performed.

---

## 🔹 **1. Price Distribution**

Shows a right-skewed distribution — most listings fall below **$200**.

---

## 🔹 **2. Average Price by Room Type**

| Room Type       | Avg Price |
| --------------- | --------- |
| Entire home/apt | ~ $210    |
| Private room    | ~ $90     |
| Shared room     | ~ $70     |

👉 Entire apartments are significantly more expensive.

---

## 🔹 **3. Average Price by Neighbourhood Group**

| Neighbourhood | Avg Price |
| ------------- | --------- |
| Manhattan     | ~ $200    |
| Brooklyn      | ~ $125    |
| Staten Island | ~ $115    |
| Queens        | ~ $100    |
| Bronx         | ~ $85     |

👉 Manhattan is the premium district.

---

## 🔹 **4. Top 10 Most Expensive Neighbourhoods**

Includes:

* Fort Wadsworth
* Woodrow
* Tribeca
* Battery Park City
* NoHo

These neighbourhoods range from **$350–$800+**.

---

## 🔹 **5. Correlation Heatmap**

* Price shows **weak correlation** with all numeric variables.
* Reviews per month ↔ number of reviews = **0.59** (expected).

➡️ **Price depends on categorical & geographical factors — not numeric ones.**

---

## 🔹 **6. Geospatial Price Map**

Latitude–Longitude scatterplot shows:

* High-priced listings concentrated in **Manhattan**.
* Outer boroughs have lower pricing.

---

# 🏁 **8. Final Conclusion**

This EDA shows that Airbnb pricing in NYC is primarily influenced by **location and room type**, not numerical features like reviews or availability.

### ✔ Strong price drivers:

* Room Type
* Neighbourhood Group
* Specific Neighbourhood
* Geographic proximity to central Manhattan

### ✘ Weak or no impact:

* Minimum nights
* Number of reviews
* Availability
* Numeric coordinates (without clustering)

### **Business Recommendations:**

* Hosts should optimize pricing based on borough/area.
* Investors should target high-value neighbourhoods like Tribeca & NoHo.
* Private/entire apartments remain the most profitable.
* Encouraging reviews improves listing visibility.

The project delivers complete insights useful for:

* Hosts
* Investors
* Analysts
* Airbnb platform teams

---

