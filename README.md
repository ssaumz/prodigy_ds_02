# README: Task-02 - Data Science Internship at Prodigy InfoTech

## Project Overview

Excited to announce the successful completion of Task-02 during my data science internship at Prodigy InfoTech 🚀. This project involved performing data cleaning and exploratory data analysis (EDA) on a dataset using Python in Jupyter Notebook. The goal was to explore relationships between variables and identify patterns and trends.

## Table of Contents

1. [Project Description](#project-description)
2. [Technologies Used](#technologies-used)
3. [Setup and Installation](#setup-and-installation)
4. [Usage](#usage)
5. [Project Structure](#project-structure)
6. [License](#license)
7. [Contributors](#contributors)

## Project Description

Task-02 focused on data cleaning and exploratory data analysis (EDA) to derive insights from a dataset. The process included handling missing values, converting categorical variables, dropping irrelevant columns, visualizing data distributions and examining survival rates.

### Objectives

- Clean the dataset by handling missing values, converting categorical variables, and dropping irrelevant columns.
- Perform exploratory data analysis to understand the data and uncover patterns and trends.
- Visualize distributions, survival rates.

## Technologies Used

- **Python**: Programming language used for data manipulation and analysis.
- **Jupyter Notebook**: Interactive computing environment for writing and running code.
- **Pandas**: Data manipulation library.
- **NumPy**: Numerical computing library.
- **Matplotlib**: Visualization library for creating static plots.
- **Seaborn**: Statistical data visualization library based on Matplotlib.

## Setup and Installation

### Prerequisites

Ensure you have the following software installed:

- Python (version 3.6 or higher)
- Jupyter Notebook

### Installation Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/username/prodigy-infotech-task-02.git
   cd prodigy-infotech-task-02
   ```

2. **Create a Virtual Environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install Required Packages**

   ```bash
   pip install -r requirements.txt
   ```

### Running the Notebook

1. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Open the notebook file `Task-02-EDA.ipynb` and run the cells sequentially.

## Usage

### Example Usage

The notebook provides a step-by-step guide on how to:

1. Load and clean the dataset.
2. Handle missing values.
3. Convert categorical variables to numerical values.
4. Drop irrelevant columns.
5. Visualize data distributions and survival rates.

#### Handling Missing Values

```python
import pandas as pd

# Load dataset
data = pd.read_csv('data/dataset.csv')

# Fill missing values
data.fillna(method='ffill', inplace=True)
```

#### Converting Categorical Variables

```python
# Convert categorical variables to numerical values
data['gender'] = data['gender'].map({'male': 0, 'female': 1})
```

#### Dropping Irrelevant Columns

```python
# Drop irrelevant columns
data.drop(columns=['irrelevant_column'], inplace=True)
```

#### Visualizing Distributions

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Plot distribution of ages
sns.histplot(data['age'], bins=10, kde=True)
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()
```

#### Visualizing Survival Rates

```python
# Plot survival rates by gender
sns.barplot(x='gender', y='survived', data=data)
plt.title('Survival Rates by Gender')
plt.xlabel('Gender')
plt.ylabel('Survival Rate')
plt.show()
```

#### Generating a Correlation Heatmap

```python
# Generate correlation heatmap
corr_matrix = data.corr()
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
plt.title('Correlation Heatmap')
plt.show()
```

## Project Structure

```
prodigy-infotech-task-02/
├── data/
│   └── dataset.csv  # Sample dataset
├── images/
│   └── age_distribuition.png  # Example of generated heatmap
├── prodigy_ds_02.ipynb  # Jupyter Notebook file
└── README.md  # Project documentation
```

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Contributors

- **Saumya Poojari** - [saumya.poojarii7@gmail.com]
- LinkedIn - https://www.linkedin.com/in/ssaumz/

Feel free to reach out with any questions or feedback!

---

Thank you for your interest in this project. Happy coding! 🚀
