# Hospital Analytics Dashboard

A full-stack data analytics and machine learning project built with Python and Streamlit that provides actionable healthcare insights through interactive visualizations, KPI tracking, and predictive modeling.

# Project Overview

This project simulates a real hospital environment with synthetic data and delivers end-to-end analytics — from raw data generation to ML-based readmission prediction — all visualized through an interactive web dashboard.

# Project Structure

hospital-analytics/
│
├── data/                          # Auto-generated CSV datasets
│   ├── patients.csv
│   ├── admissions.csv
│   ├── billing.csv
│   └── doctors.csv
│
├── hospital_data.py               #  Data generation script
├── ead.py                         #  Exploratory Data Analysis (EDA)
├── hospital_operation_kpi.py      #  KPI computation script
├── readmission_prediction.py      #  ML prediction models
├── app.py                         #  Streamlit dashboard (main app)
└── README.md

# Features

<img width="766" height="698" alt="image" src="https://github.com/user-attachments/assets/c720f35f-cf05-4a5e-97bd-db3e163cda0f" />

# Machine Learning

Logistic Regression and Random Forest Classifier for 30-day readmission prediction

Feature engineering from patient demographics, clinical, and billing data

Model comparison using ROC-AUC score

Feature importance analysis

# Dataset Overview
Synthetic data generated with numpy seed 42 for reproducibility:

<img width="766" height="405" alt="image" src="https://github.com/user-attachments/assets/05dcdde6-dc6e-4147-a50e-e9b109a5d94e" />

# ML Model Results

Target: readmitted_30_days (binary classification)

Features used: Age, Gender, Chronic Conditions, Admission Type, Department, Bed Type, Length of Stay, Insurance

<img width="769" height="278" alt="image" src="https://github.com/user-attachments/assets/a2b08f48-2de7-4c21-b632-6c7a16246d7b" />

# Key KPIs Tracked

Total Admissions & Unique Patients

Average Length of Stay (LOS)

30-Day Readmission Rate

ICU Bed Utilization %

Revenue by Department

Insurance Coverage & Claim Approval Rate

Doctor Workload (avg patients per doctor)

## Installation and Setup

Follow these steps to run the Hospital Analytics Dashboard on your local machine.

### Prerequisites

Before starting, make sure you have installed:

- Python 3
- Git
- A code editor such as Visual Studio Code

### Step 1: Clone the Repository

Open a terminal or Command Prompt and run:

```bash
git clone https://github.com/suyashitiwari4/Smart_Hospital_Analytics.git
```

Navigate to the project directory:

```bash
cd Smart_Hospital_Analytics
```

### Step 2: Create a Virtual Environment

Creating a virtual environment helps keep project dependencies separate from other Python projects.

**Windows:**

```bash
python -m venv venv
venv\Scripts\activate
```

**macOS/Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Dependencies

Install the Python packages required by the project:

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

Make sure the repository contains a `requirements.txt` file listing the project's dependencies. If it does not, add one containing the packages actually used by the project.

### Step 4: Generate the Dataset

If the CSV datasets are not already included in the repository, run the data generation script:

```bash
python hospital_data.py
```

This script generates synthetic hospital datasets, including patient, admission, billing, and doctor records. Check the script to confirm where the files are saved.

### Step 5: Run the Dashboard

Start the Streamlit application:

```bash
streamlit run app.py
```

Streamlit should open the dashboard in your browser. If it does not, open the local URL displayed in the terminal.

### Troubleshooting

- **Python is not recognized:** Check that Python is installed and available in your system PATH.
- **Module not found:** Activate the virtual environment and install the dependencies.
- **CSV file not found:** Generate the datasets and check that the file paths match those expected by the scripts.
- **Streamlit command not found:** Run `python -m pip install streamlit` in the active environment, or install the project's full requirements.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make and test your changes.
4. Commit and push your changes to your fork.
5. Open a pull request describing your contribution.

Please provide clear descriptions of bug fixes, improvements, and documentation updates.

 # Conclusion
 
This project demonstrates a complete data science pipeline applied to the healthcare domain — from synthetic data generation and EDA to interactive dashboarding and machine learning. It reflects practical skills in data engineering, visualization, and predictive analytics, simulating real-world hospital operations monitoring.




