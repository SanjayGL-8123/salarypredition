# Salary Prediction Model 💼📈

A machine learning project built with Python and scikit-learn to predict employee salary based on years of experience using Linear Regression.

---

## 📌 Project Overview

This repository demonstrates an end-to-end Simple Linear Regression workflow:
1. **Model Training**: Reads historical experience and salary data, fits a linear regression model, and serializes the trained model using `joblib`.
2. **Inference / Prediction**: Loads the trained model, accepts user input for years of experience via terminal/CLI, predicts the expected salary, and exports results to CSV.

---

## 📁 Repository Structure

```text
salarypredition/
│
├── data.csv                 # Training dataset (Years vs Salary)
├── trainning.py             # Script to train and save the linear regression model
├── salary_model.pkl         # Serialized trained machine learning model
├── predition.py             # Script to load model, take user input, and predict salary
├── predicted_salaries.csv   # Output CSV containing recent predictions
└── README.md                # Project documentation
```

---

## 📊 Dataset Details

The dataset (`data.csv`) contains historical data mapping professional experience to compensation:

| Feature | Type | Description |
| :--- | :--- | :--- |
| `Years` | Numerical (Float/Int) | Years of work experience (Independent variable / $X$) |
| `Salary` | Numerical (Float/Int) | Salary amount (Dependent target variable / $y$) |

---

## ⚙️ Prerequisites & Installation

### 1. Clone the repository
```bash
git clone https://github.com/SanjayGL-8123/salarypredition.git
cd salarypredition
```

### 2. (Optional) Create and activate a virtual environment
- **Windows (PowerShell):**
  ```powershell
  python -m venv venv
  .\venv\Scripts\Activate.ps1
  ```
- **macOS / Linux:**
  ```bash
  python3 -m venv venv
  source venv/bin/activate
  ```

### 3. Install dependencies
Install the required Python packages using pip:
```bash
pip install pandas scikit-learn joblib
```

---

## 🚀 How to Run

### Step 1: Train the Model
Run `trainning.py` to fit the Linear Regression model on `data.csv` and export `salary_model.pkl`:

```bash
python trainning.py
```

**Expected Output:**
```text
Model trained and saved as salary_model.pkl
```

### Step 2: Make Salary Predictions
Run `predition.py` to test the model with custom experience values:

```bash
python predition.py
```

**Interactive Prompt Example:**
```text
enter your experience in years: 5.5
[52500.]
Predictions saved to predicted_salaries.csv
```

The output will automatically be saved to `predicted_salaries.csv`.

---

## 🧠 Technologies Used

- **Python 3**
- **Pandas** — Data manipulation and CSV handling
- **scikit-learn** — Linear Regression model implementation
- **Joblib** — Model serialization and deserialization

---

## 👤 Author

Developed by [Sanjay G L](https://github.com/SanjayGL-8123).
