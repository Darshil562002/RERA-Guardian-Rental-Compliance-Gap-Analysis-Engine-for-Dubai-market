# RERA Guardian: Rental Compliance & Gap Analysis Engine

**RERA Guardian** is a data science and analytics project designed to monitor the Dubai rental market for "Shadow Inflation"—the discrepancy between official RERA (Real Estate Regulatory Agency) rent limits and actual market asking prices.

## Project Overview

This repository contains a comprehensive Jupyter Notebook that simulates an end-to-end data pipeline:

1.  **Data Simulation**: Generates synthetic datasets for:
    *   **Legal Baseline**: RERA calculator proxies for various zones (Business Bay, Marina, etc.).
    *   **Market Listings**: Realistic rental listings with "greedy" pricing in overheated zones.
    *   **Social Sentiment**: Simulated Reddit discussions analyzed using NLP.
2.  **Data Engineering**: Uses **SQLite** to model the data and **SQLAlchemy/Pandas** for ETL (Extract, Transform, Load) processes.
3.  **Analytics**: Calculates "Compliance Gaps" and flags high-risk buildings.
4.  **Visualization**: Interactive **Plotly** charts and a built-in **Dash** application ("Negotiation Cockpit").

## Installation & Usage

1.  **Clone the repository**:
    ```bash
    git clone <repo-url>
    cd rera-guardian
    ```

2.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Notebook**:
    ```bash
    jupyter notebook RERA_Guardian.ipynb
    ```

4.  **Explore the Dashboard**:
    Run all cells in the notebook. The final cell launches an inline Dash app where you can explore compliance heatmaps and check if a specific rent ask is fair.

## Key Technologies

*   **Python 3.8+**
*   **Pandas & NumPy**: Data manipulation.
*   **SQLite**: Local relational database.
*   **HuggingFace Transformers**: NLP for sentiment analysis.(distilbert/distilbert-base-uncased-finetuned-sst-2-english)
*   **Plotly & Dash**: Interactive visualizations and dashboarding.

## Disclaimer

This project uses **synthetic data** for demonstration purposes. It is not connected to the official Dubai Land Department (DLD) or RERA APIs.
