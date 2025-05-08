# 🏆 Yellow Taxi Trips Analytics

This project involves designing and deploying a complete ELT pipeline on Google Cloud Platform, automating data ingestion, storage, and transformation to power cloud-based analytics.

## 🧱 Architecture
![Architecture pipeline](./archi_elt.png)

### Steps in the pipeline
1. **Extraction**  
   ↳ Downloads the parquet files from a website and places them in the GCS bucket.

2. **Upload**  
   ↳ Triggers the automatic upload of files to BigQuery in a **raw table**.

3. **Transform**  
   ↳ Applies SQL or Python processing to create a **transformed table**.

## 🛠️ Technology used

| Tool / Service | Role
|-----------------------|----------------------------------|
| **Google Cloud Platform (GCP)** - Cloud platform used to host services
| **Airflow (via Google Composer)**| Orchestration of ETL tasks |
| **Google Cloud Storage (GCS)** | Storage of raw files (staging area) |
| **BigQuery** | Data warehousing and transformations |
| **Python / SQL** scripts and transformation queries
| **Parquet** | Source file format |


## 💻​ Environment setup

1. Clone the repository

In your terminal,
```sh
git clone https://github.com/Desy16/yellow-taxi-trips-analytics.git
cd yellow-taxi-trips-analytics
```

2. Create and activate a virtual environment
```sh
python3 -m venv .venv
source .venv/bin/activate
```

3. Install dependencies
```sh
pip install -r requirements.txt
```

## 🧰​ Dependencies
```txt
google==3.0.0
google-api-core==2.24.1
google-auth==2.38.0
google-cloud==0.34.0
google-cloud-bigquery==3.29.0
google-cloud-core==2.4.1
google-cloud-storage==3.0.0
numpy==2.2.2
pandas==2.2.3
py4j==0.10.9.7
pyarrow==19.0.0
scikit-learn==1.6.1
```

## 👨‍💻​ Author
[Desty MPASSI MATONDO](https://github.com/DestyM/)