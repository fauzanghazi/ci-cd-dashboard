# 🧩 CI/CD Dashboard – Data Cleaning & Visualization

This project demonstrates a simple yet effective **CI/CD pipeline for data preprocessing and dashboard visualization** using **GitHub Actions**, **Python**, and **Streamlit**.  
It automatically validates code, removes duplicate rows from a dataset, and provides an interactive dashboard for stakeholders to explore processed data.

---

## 🚀 Features

- **Automated Data Cleaning**  
  - Removes duplicate rows and saves a clean dataset.  
  - Generates a summary report of transformations.  

- **CI/CD Integration**  
  - GitHub Actions pipeline automatically installs dependencies and runs tests on every push or pull request to `main`.  
  - Ensures the project is always in a deployable state.

- **Interactive Dashboard**  
  - Built with Streamlit to visualize the cleaned dataset.  
  - Includes search and filter functionality for stakeholder insights.

- **Automated Testing**  
  - Pytest ensures data integrity (no duplicates after processing).

---
## 🧱 Structure

```text
ci-cd-dashboard/
│
├── .github/
│   └── workflows/
│       └── ci_cd_pipeline.yml       # GitHub Actions workflow
│
├── data/
│   ├── dataset.csv                  # Raw dataset
│   ├── processed_dataset.csv        # Cleaned dataset (auto-generated)
│   └── summary_report.txt           # Transformation summary
│
├── src/
│   ├── main.py                      # Data extraction and cleaning
│   └── dashboard.py                 # Streamlit visualization app
│
├── tests/
│   └── test_no_duplicates.py        # Pytest for duplicate removal
│
├── requirements.txt                 # Python dependencies
└── README.md                        # Project documentation

