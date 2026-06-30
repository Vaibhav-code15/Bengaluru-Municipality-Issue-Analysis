# 🏙️ Bengaluru Municipality Issue Analysis

> Exploratory Data Analysis on 16,071 civic complaints submitted to Bengaluru Municipality between 2019 and 2022 via the **I Change My City** platform by Janaagraha.

---

## 📌 Project Overview

This project performs a structured EDA on citizen-reported complaints to understand:
- What issues Bengaluru citizens complain about the most
- Which civic agencies handle the most complaints
- How effectively complaints are being resolved
- How complaint volumes have changed over time (2019–2022)
- Which wards are the most underserved

The analysis was done as part of a data analyst internship assignment and is also published as a standalone portfolio project.

---

## 📊 Key Findings

| # | Finding |
|---|---------|
| 1 | **Roads & Infrastructure** is the #1 complaint category at ~32% of all complaints |
| 2 | **Garbage & Unsanitary Practices** follows at ~25% — together these two = over 55% of all complaints |
| 3 | **BBMP handles 83%+** of all complaints — roads, garbage, streetlights all under one agency |
| 4 | Only **30.7% of complaints are marked Resolved** — over 54% remain Open, signalling a large backlog |
| 5 | **2.1% of complaints were Re-opened** after closure — meaning some resolutions were not acted upon |
| 6 | Complaints declined **79%** from 7,383 (2019) to 1,551 (2022) — steepest drop in 2020 coincides with **COVID-19 lockdowns** |
| 7 | Complaint activity is concentrated in a **few wards** — clear hotspots for targeted resource allocation |

---

## 🗂️ Project Structure

```
blr-municipality-eda/
│
├── data/
│   └── a60abf5c-3a15-4967-af32-c3074248580f.csv   ← Raw dataset (download separately)
│
├── BLR_Municipality_Issue_Analysis.ipynb            ← Main EDA notebook
├── BLR_Municipality_EDA_Slides.pptx                 ← Summary presentation (3 slides)
├── requirements.txt                                 ← Python dependencies
└── README.md                                        ← You are here
```

---

## 📁 Dataset

| Field | Details |
|-------|---------|
| **Source** | [OpenCity — data.opencity.in](https://data.opencity.in/dataset/i-change-my-city-data/resource/a60abf5c-3a15-4967-af32-c3074248580f) |
| **Platform** | I Change My City — Janaagraha |
| **Period** | January 2019 – December 2022 |
| **Records** | 16,071 complaints |
| **Columns** | 17 (category, sub-category, ward, agency, status, date, location, comments etc.) |

> ⚠️ The dataset is not included in this repository. Download it directly from the OpenCity link above and place it inside the `data/` folder before running the notebook.

---

## 🔍 Notebook Structure

The notebook is organized into 12 sections:

| Section | Description |
|---------|-------------|
| 1 | Import Libraries |
| 2 | Load Dataset |
| 3 | Dataset Overview |
| 4 | Data Quality Assessment (Missing Values & Duplicates) |
| 5 | Feature Engineering (Date Parsing) |
| 6 | Complaint Category & Sub-issue Analysis |
| 7 | Complaint Status Analysis |
| 8 | Civic Agency Analysis |
| 9 | Ward-Level Analysis |
| 10 | Complaint Trend Analysis (Year & Month) |
| 11 | Key Insights |
| 12 | Conclusion |

---

## 🚀 How to Run This Project

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/blr-municipality-eda.git
cd blr-municipality-eda
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Download the Dataset

Go to: [https://data.opencity.in/dataset/i-change-my-city-data](https://data.opencity.in/dataset/i-change-my-city-data)

Download the CSV file and place it inside the `data/` folder:

```
data/a60abf5c-3a15-4967-af32-c3074248580f.csv
```

### 4. Update the File Path

Open `BLR_Municipality_Issue_Analysis.ipynb` and update the file path in **Section 2** to match your local path:

```python
# Update this line with your actual file path
issues = pd.read_csv(r"data/a60abf5c-3a15-4967-af32-c3074248580f.csv")
```

### 5. Run the Notebook

```bash
jupyter notebook BLR_Municipality_Issue_Analysis.ipynb
```

Run all cells top to bottom (`Kernel → Restart & Run All`).

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python 3.x | Core programming language |
| Pandas | Data loading, cleaning and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical charts |
| Jupyter Notebook | Interactive development environment |

---

## 📽️ Presentation

A 3-slide summary presentation (`BLR_Municipality_EDA_Slides.pptx`) is included in this repository covering:
- **Slide 1** — Project overview and key stats
- **Slide 2** — What citizens are complaining about (category + agency breakdown)
- **Slide 3** — Complaint trends and key findings

---

## 👤 Author

**[Your Name]**  
[LinkedIn](https://linkedin.com/in/yourprofile) · [GitHub](https://github.com/yourusername)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> *Data Source: I Change My City — Janaagraha · [OpenCity](https://data.opencity.in)*
