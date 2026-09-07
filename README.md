# BA-T8 — Urban Tree Species Distribution & Contribution Dashboard

## 📊 Project Overview

This project uses **Tableau Public** to analyze the distribution, contribution, and physical characteristics of urban tree species using an interactive dashboard.

The analysis focuses on identifying the tree categories, common species, geographic areas, and growing spaces that contribute the most to the overall urban tree population.

Although the source dataset is not a traditional sales or revenue dataset, the project follows the same contribution-analysis approach by using **tree count as the primary numerical measure** and supporting measures such as **Diameter at Breast Height (DBH), Height, and Width**.

---

## 🎯 Objective

To analyze the contribution of different tree categories and species using a **Tree Map in Tableau** and identify the categories, species, locations, and growing environments that have the greatest impact on the overall urban tree inventory.

---

## ❓ Problem Statement

Using the provided **Tree Species dataset**, create an interactive Tableau dashboard to:

- Compare the contribution of different tree categories and common species.
- Identify the areas with the highest tree populations.
- Examine the relationship between tree height and trunk diameter.
- Analyze how trees are distributed across different growing spaces.
- Generate useful analytical insights and recommendations from the dashboard.

---

## 📁 Dataset

**Dataset:** `Tree_Species.csv`

The dataset contains information related to urban trees, including:

- Tree Category
- Common Name
- Area
- Grow Space
- Height
- Width
- Diameter at Breast Height
- Object ID / Tree Record

### Main Fields Used

| Purpose | Field |
|---|---|
| Main Category | `TreeCategory` |
| Sub-Category | `CommonName` |
| Tree Count | `CNT(OBJECTID)` |
| Tree Diameter | `AVG(DiameterAtBreastHeight)` |
| Geographic Analysis | `Area` |
| Growing Environment | `GrowSpace` |
| Tree Height | `Height` |
| Tree Width | `Width` |

---

## 📈 Tableau Visualizations

### 1. Tree Map — Tree Population Contribution

The Tree Map compares the contribution of different tree species and categories.

- **Size:** `CNT(OBJECTID)`
- **Colour:** `AVG(DiameterAtBreastHeight)`
- **Label:** `CommonName` and tree count
- **Detail:** `TreeCategory`

Larger blocks represent species with a greater number of recorded trees, while colour helps compare their average trunk diameter.

### 2. Tree Distribution by Area

A horizontal bar chart compares the number of recorded trees across different geographic areas.

- **Rows:** `Area`
- **Columns:** `CNT(OBJECTID)`

This visualization helps identify the areas containing the largest urban tree populations.

### 3. Tree Height vs Diameter by Species

A scatter plot is used to examine the relationship between tree height and Diameter at Breast Height.

- **X-Axis:** `AVG(DiameterAtBreastHeight)`
- **Y-Axis:** `AVG(Height)`
- **Detail:** `CommonName`
- **Size:** `CNT(OBJECTID)`

This chart helps identify species that are generally taller, wider, or more mature.

### 4. Tree Distribution by Growing Space

A bar chart compares the number of trees found in different growing environments.

- **Category:** `GrowSpace`
- **Measure:** `CNT(OBJECTID)`

This helps determine which types of growing spaces support the largest proportion of the urban tree population.

---

## 🧩 Dashboard Features

The final Tableau dashboard combines all four visualizations into a single interactive analytical view.

Interactive filters include:

- Area
- Tree Category
- Common Name

These filters allow users to explore specific geographic areas, categories, and species while automatically updating the related visualizations.

---

## 🔎 Key Insights

1. **Park Trees are the largest tree category**, containing approximately **13,906 trees**, or around **41% of the total inventory**.

2. **Garry Oak is the most frequently recorded tree species**, with approximately **4,776 trees**, followed closely by **Cherry Plum** with around **4,397 trees**.

3. **Fairfield and James Bay have the largest tree populations**. Together they account for approximately **40% of all recorded trees** in the dataset.

4. There is a **strong positive relationship between tree height and Diameter at Breast Height**, indicating that trees with larger trunks generally tend to be taller and more mature.

5. Approximately **73% of the recorded trees are located in Turf growing spaces**, making Turf the dominant growing environment in the dataset.

---

## 💡 Recommendations

### 1. Improve Species and Location Diversity

Because a large portion of the inventory is concentrated among a few tree categories and common species, future planting programs should encourage greater species and location diversity. This can improve long-term resilience and reduce dependence on a small number of dominant species.

### 2. Prioritize High-Density Areas for Maintenance

Areas such as **Fairfield and James Bay** contain a major share of the total tree population. These locations should receive greater attention in inspection, pruning, maintenance, and long-term urban forestry planning.

---

## 🧹 Data Preparation

Before creating the visualizations, the dataset was reviewed for missing and unrealistic values.

For physical-measure analysis, records with invalid values such as negative heights or widths should be excluded where appropriate so that they do not distort the scatter plot and summary statistics.

---

## 🛠️ Tools Used

- **Tableau Public** — Dashboard development and visualization
- **CSV Dataset** — Source data
- **GitHub** — Project documentation and version control

---

## 🌐 Live Tableau Dashboard

👉 **[View the Urban Tree Species Distribution & Contribution Dashboard on Tableau Public](https://public.tableau.com/app/profile/santhosh.v2k7/viz/UrbanTreeSpeciesDistributionContributionDashboard/UrbanTreeSpeciesDistributionContributionDashboard?publish=yes)**

---

## 📌 Project Summary

This project demonstrates how Tableau can be used to transform a large categorical dataset into an interactive dashboard. The Tree Map provides a clear view of species contribution, while the supporting bar charts and scatter plot reveal geographic concentration, growing-space distribution, and relationships between physical tree characteristics.

The dashboard makes it easier to identify dominant species, high-density areas, and important patterns that can support better urban tree-management decisions.

---

## 👤 Author

**Santhosh V**

Business Analytics — Task 8 (BA-T8)
