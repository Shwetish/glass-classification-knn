# Glass Type Classification using KNN
An end-to-end Machine Learning pipeline using K-Nearest Neighbors (KNN) to automate glass type classification for manufacturing plants based on chemical and physical properties.

## 1. Business Problem
### 1.1 Business Objective
A glass manufacturing plant uses different earth elements to design new glass materials based on specific customer requirements. Manually classifying these glass types is tedious, error-prone, and time-consuming. The objective is to automate the classification process using machine learning to accurately categorize glass types based on their chemical and physical attributes.

### 1.2 Constraints
* High classification accuracy is critical because misclassifying structural or specialized glass can lead to product failure or safety hazards.
* Inference time should remain low for real-time manufacturing line integration.

---

## 2. Data Dictionary
| Feature Name | Data Type | Relevance | Description / Reason for Inclusion/Exclusion |
| :--- | :--- | :--- | :--- |
| `Id` | Integer | Irrelevant | Index/identifier column; dropped prior to model building. |
| `RI` | Float | Relevant | Refractive index; key chemical property reflecting material composition. |
| `Na` | Float | Relevant | Sodium content (unit measurement in weight percent). |
| `Mg` | Float | Relevant | Magnesium content; vital for structural stability. |
| `Al` | Float | Relevant | Aluminum content affecting durability. |
| `Si` | Float | Relevant | Silicon content as the primary matrix element. |
| `K` | Float | Relevant | Potassium content. |
| `Ca` | Float | Relevant | Calcium content. |
| `Ba` | Float | Relevant | Barium content. |
| `Fe` | Float | Relevant | Iron content. |
| `Type` | Integer | Target | Target variable indicating the glass classification category. |

---

## 3. Exploratory Data Analysis (EDA)
* **Summary:** Analyzed missing values, data distributions, and feature scales.
* **Univariate Analysis:** Inspected feature distributions using histograms and boxplots to identify skewed features and outliers.
* **Bivariate Analysis:** Generated correlation heatmaps to detect multicollinearity among chemical elements (e.g., Refractive Index vs. Calcium).

---
