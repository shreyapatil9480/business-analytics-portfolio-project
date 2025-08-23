# Business Analytics Portfolio Project

This repository contains a self‑contained project designed for business analysts, program managers and data analysts looking to showcase their analytical skills.  The project uses a **synthetic dataset** that simulates monthly business metrics for a hypothetical company.  It is ready to run out of the box and includes everything needed to explore, visualize and model the data.

## Project overview

The goal of this project is to perform end‑to‑end data analysis on a fictitious set of business data.  You will:

1. **Load a synthetic dataset** containing 36 months of business metrics such as marketing spend, product development cost, customers acquired, revenue, net promoter score, support tickets and churn rate.
2. **Perform exploratory data analysis (EDA):**
   * View summary statistics and inspect distributions.
   * Plot time series of revenue and marketing spend.
   * Compute and visualize a correlation matrix to identify relationships between variables.
3. **Build predictive models of increasing complexity:**
   * **Linear Regression** to predict revenue using marketing spend, product development cost and customers acquired (suitable for an entry‑level analyst).
   * **Random Forest Regression** to predict churn rate using multiple features (a more advanced modelling technique).
4. **Interpret results** by examining metrics such as mean squared error (MSE), \(R^2\) and feature importance.

The analysis is provided in a Jupyter notebook (`business_analytics_project.ipynb`) and can be run step by step.  The notebook includes narrative text explaining each section and code cell.

## Dataset

File: `synthetic_business_data.csv`

This dataset was generated synthetically to mimic real‑world business behaviour.  Each row represents a single month from January 2021 onward.  Columns include:

| Column | Description |
|-------|-------------|
| `date` | Month (YYYY‑MM‑DD) |
| `marketing_spend` | Marketing spend in USD |
| `product_development_cost` | Product development cost in USD |
| `customers_acquired` | Number of new customers acquired |
| `revenue` | Revenue generated in USD |
| `net_promoter_score` | Net promoter score (0–100) |
| `support_tickets` | Number of support tickets received |
| `churn_rate` | Customer churn rate (%) |

All numbers have been randomly generated with realistic relationships and noise; they do **not** reflect any real company data.

## Getting started

These instructions will help you set up a local environment, install dependencies and run the analysis.

### Prerequisites

Ensure you have Python 3.8+ installed on your machine.  You will also need `pip` for installing packages.

### Clone the repository

```bash
git clone https://github.com/<your‑username>/<repository‑name>.git
cd <repository‑name>
```

Replace `<your‑username>` and `<repository‑name>` with your GitHub username and this repository’s name.

### Install dependencies

Create a virtual environment (recommended) and install required packages using the provided `requirements.txt` file:

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

pip install -r requirements.txt
```

### Run the notebook

Launch Jupyter Notebook or JupyterLab and open the analysis notebook:

```bash
jupyter notebook business_analytics_project.ipynb
# or
jupyter lab business_analytics_project.ipynb
```

Follow the notebook step by step.  Each section explains what it is doing and includes code and visualizations.

## File structure

```
.
├── README.md                  – This overview and instructions
├── requirements.txt           – Python dependencies
├── synthetic_business_data.csv – Synthetic dataset used for analysis
├── business_analytics_project.ipynb – Jupyter notebook with EDA and models
```

## Contributing

If you wish to extend this project (for example by adding new features, experimenting with different algorithms, or improving the visualizations), feel free to fork the repository and submit a pull request.  Suggestions and improvements are welcome!

## License

This project is provided under the MIT License.  See the `LICENSE` file for details.

