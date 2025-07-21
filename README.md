# 🧾 Service Quality Assessment of Orange Line Metro Train

This dataset is a result of a public survey conducted to evaluate the **service quality** of the **Orange Line Metro Train in Lahore, Pakistan**. The survey includes various questions related to passenger satisfaction, cleanliness, safety, accessibility, punctuality, and overall service experience.

## 📁 Dataset Information

- **File name**: `Service.csv`
- **Size**: Small (< 1MB)
- **Records**: Multiple rows, each representing a survey response.
- **Target Column**: 
  - `How satisfied are you with the overall service quality of the Orange Line Metro Train?` (Rating scale: 1 = Best to 5 = Worst)

### 📌 Features Include:
- Demographics (e.g., Age, Gender)
- Travel purpose and frequency
- Accessibility and safety concerns
- Ticketing and fare opinions
- Facility-related feedback (cleanliness, announcements, platform)
- Final satisfaction rating (Target variable)

---

## 🔍 How to Use the Dataset

### 1️⃣ Exploratory Data Analysis (EDA)
Use pandas and seaborn/matplotlib to:
- Check class distributions
- Analyze individual feature trends (e.g., Age vs Satisfaction)
- Detect missing values or outliers
- Create boxplots, histograms, and correlation heatmaps

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

df = pd.read_csv("Service.csv")
sns.countplot(x='How satisfied are you with the overall service quality of the Orange Line Metro Train?', data=df)
plt.show()
