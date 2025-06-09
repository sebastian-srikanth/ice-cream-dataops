# Cognite Bootcamp: Ice Cream DataOps

Welcome! This repository is your hands-on guide to using Cognite Data Fusion (CDF) tools end-to-end. You’ll learn how to onboard data, contextualize assets with timeseries, calculate OEE, orchestrate workflows, and use industrial analytics tools—all with real examples from the Ice Cream API.

---

## 🚀 How to Start

1. **Read the [Bootcamp Documentation](https://docs.cdf-bootcamp.cogniteapp.com)**  
   The official docs walk you through every step, from setup to advanced analytics.

2. **Install Prerequisites**
   - [Cognite Python SDK](https://cognite-sdk-python.readthedocs-hosted.com/en/latest/)
   - A valid CDF `.toml` config file with your project and authentication details

3. **Follow the Steps**
   - **Data Onboarding:** Connect to the Ice Cream API and ingest data into CDF.
   - **Data Contextualization:** Link assets with timeseries data for a digital twin.
   - **OEE Calculation:** Define and compute Overall Equipment Effectiveness (OEE).
   - **Orchestration:** Automate workflows using CDF Workflows.
   - **Industrial Tools:** Visualize and analyze your data using CDF’s industrial apps.

---

## 📦 Key Modules in This Repo

- **Data Ingestion:** Scripts/configs for onboarding data from the Ice Cream API.
- **Transformations:** Contextualize assets and timeseries, and perform OEE calculations.
- **Workflows:** Automate data pipelines and processes using CDF Workflows.

---

## ⚠️ Important Steps & Missing Points from Bootcamp Docs

- **Before deploying to production:**
  - Set up the `cognite_toolkit_service_principal` for the production environment.
  - Ensure the `oidc-admin-group` has these permissions:
    1. Workflows (full access)
    2. Extractors (full access)
    3. Functions
    4. Data Models & Data Model Instances
    5. Data Sets
    6. RAW
    7. Transformations
    8. Sessions (to run Functions)
    9. Monitoring
    10. Timeseries

- **Run Create Cognite Asset Hierarch Transformation:**  
  Before Verifying we have 1021 Assets, run the transformation **Create Cognite Asset Hierarchy** and verify you have **1021 assets**.  
  [See details](https://docs.cdf-bootcamp.cogniteapp.com/content/data_modeling/gitHub_prod/#verify-in-the-ui)

- **Charts App:**  
  When working with charts, use **Create Calculation** (not "Add calculation").  
  [See details](https://docs.cdf-bootcamp.cogniteapp.com/content/industrial_tools/visualize_and_validate_data_in_charts/#exercise)

- **Industrial Canvas:**  
  Before adding data, run the transformation **Contextualize TimeSeries and Assets** that contextualizes assets with timeseries. Only then will you see related timeseries data.  
  [See details](https://docs.cdf-bootcamp.cogniteapp.com/content/industrial_tools/industrial_canvas/#create-an-industrial-canvas)

---

## 📚 More Information

- Full documentation: [https://docs.cdf-bootcamp.cogniteapp.com](https://docs.cdf-bootcamp.cogniteapp.com)
- If you spot missing steps or improvements, please open an issue or pull request!

---

**This README is designed to help anyone—new or experienced—get started quickly and avoid common pitfalls. Happy bootcamping!**