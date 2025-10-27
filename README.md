# 📊 OkCupid Dataset Analysis — EDA with Python

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/YOUR_GITHUB_USERNAME/REPO_NAME/HEAD?filepath=main.ipynb)

---

## 🗂️ Table of Contents
1. [Overview](#🧠-overview)
2. [Dataset](#📂-dataset)
3. [Objectives](#🎯-objectives)
4. [Tools & Libraries](#🧰-tools--libraries)
5. [How to Run](#⚙️-how-to-run)
6. [Results & Visuals](#📈-results--visuals)
    - [Data Cleaning & Preparation](#🧹-data-cleaning--preparation)
    - [Demographic Overview](#👥-demographic-overview)
    - [Personality & Textual Data](#💬-personality--textual-data)
    - [Interactive Visualizations](#🎨-interactive-visualizations)
    - [Static Visualizations](#📊-static-visualizations)
7. [Key Takeaways](#🧩-key-takeaways)
8. [Next Steps](#💡-next-steps)
9. [Author](#🧾-author)

---

## 🧠 Overview
This project performs an **Exploratory Data Analysis (EDA)** on the OkCupid dating dataset, focusing on **user demographics, preferences, and behavioral patterns**.  
It demonstrates **data cleaning, structuring, and visualization** using Python libraries, including both **static** and **interactive plots**.

---

## 📂 Dataset
- Approximately **60,000 user profiles**  
- 👥 Demographics: age, status, sex, orientation, body_type, diet, drinks, income...  
- 💬 Text responses from open-ended questions  
- 💡 Lifestyle and preference features  

> Dataset is for **educational and non-commercial purposes**.

---

## 🎯 Objectives
- Clean and structure the dataset for analysis  
- Explore demographic patterns and distributions  
- Create **interactive visualizations** with Holoviews + hvPlot + Bokeh  
- Complement with **static visualizations** using matplotlib and seaborn  
- Compile workflow in a reproducible **Jupyter Notebook**

---

## 🧰 Tools & Libraries

### Python Installations
```bash
pip install holoviews hvplot seaborn matplotlib pandas numpy
```

### Python Imports
```python
import pandas as pd
import numpy as np
import holoviews as hv
import seaborn as sns
import matplotlib.pyplot as plt
import hvplot.pandas
from hvplot import hvPlot

# Activate Holoviews Bokeh extension
hv.extension('bokeh')
```

**Libraries Used:**
- `pandas`, `numpy` → data manipulation  
- `matplotlib`, `seaborn` → static visualizations  
- `holoviews`, `hvplot`, `bokeh` → interactive visualizations  

---

## ⚙️ How to Run

### Locally
```bash
jupyter notebook main.ipynb
```
Make sure all libraries above are installed via `pip install`.

### Online (Binder)
[Launch Notebook on Binder](https://mybinder.org/v2/gh/AlexandraB12/okcupid-analysis/HEAD?urlpath=%2Fdoc%2Ftree%2Fmain.ipynb)

---

## 📈 Results & Visuals

<details>
<summary>🧹 Data Cleaning & Preparation</summary>

- Cleaned missing or inconsistent values  
- Structured numeric and categorical features  
- Prepared textual columns for potential NLP  

**Result:** clean, structured dataset ready for analysis

</details>

<details>
<summary>👥 Demographic Overview</summary>

- Age distribution: concentrated 25–35 years old  
- Gender & orientation ratios typical for dating apps  
- Geographic distribution visualized with interactive plots  

**Insight:** profile completion varies by age and region

</details>

<details>
<summary>💬 Personality & Textual Data</summary>

- Explored open-ended essays for themes like **travel, music, friends**  
- Essay length correlates with engagement  

**Insight:** textual openness may indicate personality and matching potential

</details>

<details>
<summary>🎨 Interactive Visualizations</summary>

```python
# Example interactive histogram
df.hvplot.hist('age', bins=30, title='Age Distribution')

# Example interactive scatter plot
df.hvplot.scatter(
    x='age',
    y='essay_length',
    by='orientation',
    size=5,
    alpha=0.6
)
```

- Multi-dimensional scatter plots with hover insights  
- Dynamic histograms for user attributes  

</details>

<details>
<summary>📊 Static Visualizations</summary>

- Histograms, bar charts, scatter plots with matplotlib/seaborn  
- Quick quantitative summaries for comparison  

</details>

---

## 🧩 Key Takeaways
- **Data cleaning & structuring** essential for accurate EDA  
- **Interactive visualizations** improve pattern exploration  
- Workflow shows **raw → clean → visual insights**  
- Combines quantitative & qualitative exploration

---

## 💡 Next Steps
- Apply **NLP sentiment analysis** on essay responses  
- Explore **clustering** for behavioral segments  
- Build **predictive compatibility model**

---

## 🧾 Author
**Alexandra Boudia**  
Data Analyst | Data Science Fullstack | AI Engineering  
📫 [[LinkedIn Profile]](https://www.linkedin.com/in/alexandra-boudia/)
