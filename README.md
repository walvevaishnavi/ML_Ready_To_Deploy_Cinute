🚀 Ready-to-Deploy Machine Learning Collection(Read-Only)

A polished collection of five production-ready ML notebooks and scripts — each built with reproducibility, clarity, and deployment in mind.

🔭 Projects included

Each notebook is a stand-alone, end-to-end mini-project: data ingestion → clean preprocessing → EDA (static + interactive) → model building → evaluation → model export for deployment.

Insurance.ipynb — Claims / premium modelling pipeline: feature engineering for categorical policy data, regression/classification baselines, model explainability notes, and a serialized model ready for API serving.

Salary_Distribution.ipynb — HR/compensation analysis: distributional analysis, outlier handling, and predictive salary-range estimation using regression ensembles.

Smart home device usage.ipynb — Time-series / usage-pattern analysis for IoT devices: sessionization, feature windows, visualization with Plotly, and anomaly-detection prototype.

Solar power gen.ipynb — Renewable energy forecasting: weather-feature fusion, lag features, model pipeline for short-term generation forecasting, and notes for edge/cloud deployment.

Wine data set.ipynb — Classic classification workflow: data cleaning, feature importance, classifier comparison, cross-validation, and model export with reproducible scoring.

✨ Why this repo is different

Deployment-first: notebooks include model serialization (.pkl/joblib) and a clear path to wrap models into Flask/FastAPI or Streamlit apps.

Interactive + static EDA: Matplotlib/Seaborn for publication-ready charts and Plotly for interactive dashboards.

Modular pipelines: code separated into preprocessing, feature engineering, modelling, and utility blocks — easy to refactor into src/ modules.

Reproducible experiments: consistent random seeds, requirements.txt, and notebook checkpoints showing metric baselines.

Practical notes: pointers for hyperparameter tuning, evaluation choices, and deployment considerations (containerization, cloud hints).

🧰 Tech stack

Python 3.8+ • Pandas, NumPy, Matplotlib, Seaborn, Plotly, Scikit-Learn, joblib
🏁 Quickstart
# 1. clone
git clone <repo-url>
cd repo-name


# 2. create venv and install
python -m venv venv
source venv/bin/activate # mac/linux
venv\Scripts\activate # windows
pip install -r requirements.txt


# 3. open notebooks
jupyter lab
# run the notebooks in order or use the exported scripts in `src/`
├── data/ # raw and processed datasets
├── notebooks/ # the five notebooks (Insurance, Salary..., etc.)
├── src/ # reusable pipeline scripts (preprocess.py, model.py)
├── models/ # exported trained models (.pkl / .joblib)
├── reports/ # visuals, metric summaries, model cards
├── requirements.txt
├── Dockerfile # optional: containerize the API
└── README.md
