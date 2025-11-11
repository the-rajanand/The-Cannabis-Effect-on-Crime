# 📊 The Cannabis Effect on Crime: Data Correlation and Research Analysis

This repository contains the code and analysis for a research project that investigates the relationship between the presence of medical marijuana dispensaries (MMDs) and neighbourhood crime rates in Los Angeles using machine learning and data mining techniques.

---

## ✨ Project Goal

The primary objective was to examine real-world data and develop a swift, efficient, and accurate model to forecast the likelihood of increased crime rates associated with the presence of medical marijuana dispensaries. The system serves as a valuable training tool for law enforcement and researchers.

---

## 🔍 Data and Features

The analysis utilizes data from multiple sources, primarily focused on the Los Angeles area:

* **Primary Crime Data:** **`Crime_Data.xlsx`** (Original LAPD data containing $\sim 1,048,575$ crime incidents).
* **Socioeconomic and Land Use Data:** Datasets like **`Cannabis_Dataset.xlsx`** and **`Crime_cannabis_dataset.xlsx`** comparing blocks *with* and *without* dispensaries using factors like Average Household Income, Percent Homeowners, and land use proportions.
* **Correlation Data:** Coefficients illustrating the linear relationship between socio-environmental factors and four key crime types (Homicide, Robbery, Assault, Burglary).

---

## 🔬 Research Analysis

This project's core contribution is its empirical analysis of the complex nexus between MMDs and crime rates:

* **Key Finding:** The research indicates an **association between the presence of medical marijuana dispensaries and an increase in neighbourhood crime rates**, particularly in socially organized blocks.
* **Contributing Factors:** This observed correlation is often linked to factors such as dispensary location in poor neighbourhoods and proximity to alcohol outlets.
* **Versatility:** The generalized system allows for seamless adaptation to various datasets by simply adjusting the input dataset file during the training module, making it a scalable tool for analysing diverse socio-environmental factors influencing crime rates.

---

## 💻 Methodology & Modeling

The methodology focused on data preprocessing (handling missing data, one-hot encoding for categorical variables) and comparative analysis using multi-output regression models.

### Algorithms Compared

Four supervised learning algorithms were implemented and their R-squared accuracies (for predicting crime rates based on dispensary presence) were compared:

| Algorithm | Best Accuracy (R-squared) | Key Characteristics |
| :--- | :--- | :--- |
| **Decision Tree** | 98.51% | Highly accurate, capable of capturing complex relationships. |
| **Random Forest** | 98.13% | Ensemble method providing better generalization by reducing overfitting. |
| **Linear Regression** | 80.53% | Assumes linear relationships; may not perform well when the underlying relationship is complex. |
| **Support Vector Machine (SVM)** | 42.14% | Struggles with capturing complex relationships or non-linear patterns in this data. |

---

## 🚀 Getting Started

Follow these steps to clone the repository, set up your environment, and run the analysis using **Jupyter Notebook**.

### Prerequisites

* **Python:** Version 3.x
* **Jupyter Notebook:** Or an IDE like VS Code with Python support.
* **Git:** Installed on your system.

### Setup Instructions

1.  **Clone the Repository**
    Open your terminal and clone the project files:
    ```bash
    git clone [https://github.com/the-rajanand/The-Cannabis-Effect-on-Crime.git](https://github.com/the-rajanand/The-Cannabis-Effect-on-Crime.git)
    cd The-Cannabis-Effect-on-Crime
    ```

2.  **Install Dependencies**
    This project requires several key Python libraries. Use the provided **`requirements.txt`** file to install them automatically:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Data Placement**
    Ensure all raw data files (`Crime_Data.xlsx`, `Cannabis_Dataset.xlsx`, etc.) are placed in the root directory of the cloned repository.

### Execution Flow

The project is executed sequentially across multiple notebooks to build and compare the models:

1.  **Initial Data Analysis:** Start with the **`LAPD Dataset Accuracies.ipynb`** file.
2.  **Feature and Model Preparation:** Run the **`The_Crimes.ipynb`** and **`With_and_Without.ipynb`** notebooks to perform feature engineering and initial model setup.
3.  **Final Modeling:** Execute the **`Final Decision Tree.ipynb`** and **`Final Accuracies.ipynb`** notebooks to train the full models and obtain the final prediction scores.
4.  **Visualization:** Run the **`Comparisons.ipynb`** notebook last to generate the visual comparison of the machine learning model accuracies.

---

## 👤 Author

* **Raj Anand**
