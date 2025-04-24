# 🧹 Data Preprocessing Pipeline – Titanic Dataset

This project demonstrates a complete data preprocessing workflow using the Titanic dataset. The goal is to prepare the data for machine learning by cleaning, transforming, and standardizing it. This includes handling missing values, encoding categorical variables, normalizing numerical features, and detecting/removing outliers.

---

## 📁 Dataset

The dataset used is the famous **Titanic passenger dataset**, which includes details such as passenger age, gender, class, fare, and survival status. It contains both categorical and numerical features and is commonly used for data analysis and machine learning practice.

---

## 🔄 Steps in the Preprocessing Pipeline

### 🔍 1. Import and Explore the Dataset

The dataset was first loaded and basic information such as column names, data types, and the presence of null values was explored. This helped to understand the structure and quality of the data before applying any transformations.

---

### 🛠️ 2. Handle Missing Values

Missing values in the dataset were handled based on the type of feature. For example, numerical columns like "Age" were filled with the **mean** of the column, while categorical columns like "Cabin" were filled using the **mode** (most frequent value).

---

### 🔤 3. Encode Categorical Features

Categorical variables such as "Sex" "Name" "Age" "Ticket" "Cabin" "Embarked" were converted into numerical format using **Label Encoding**. This transformation is essential as machine learning models work with numerical data.

---

### 📊 4. Normalize Numerical Features

Numerical features such as "Ticket" and "Fare" were standardized using **StandardScaler**. Standardization helped bring all numerical values into a common scale with a mean of 0 and standard deviation of 1, which improves model performance and training stability.

---

### 📦 5. Outlier Detection and Removal (Z-Score)

Outliers in the dataset were identified and removed using the **Z-Score** method. Boxplots were used for visualizing potential outliers in numerical features like "Fare" and "Age". Then, Z-scores were calculated, and any data points that fell beyond three standard deviations from the mean were considered outliers and removed. This step ensures a cleaner dataset by removing extreme values that could negatively impact model performance.

---

## ✅ Final Output

The final dataset is:
- Free from missing values
- Encoded for machine learning compatibility
- Standardized for numerical consistency
- Cleaned of outliers for better accuracy

This processed Titanic dataset is now ready to be used for training classification models or further analytical tasks.

---

## 📚 Requirements

This project was implemented using Python and the following libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, and `seaborn`.

---

## 👩‍💻 Author

Made with 💻 by **[Pugalenthi]**

---

## 📃 License

This project is licensed under the MIT License.
