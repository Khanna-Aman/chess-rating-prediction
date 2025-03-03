# Chess Rating Prediction - Lichess

This project predicts chess ratings using historical data from the **Lichess** website. The model is designed to handle various rating formats such as **Bullet, Blitz, Classical,** and more. It fetches rating data through the **Lichess API,** processes it, and predicts a player's future rating based on their past performance.

## Project Description

This repository contains a Jupyter Notebook that uses the **Lichess API** to fetch rating data for any user and any game format. The project can handle different rating modes, such as Bullet, Blitz, Classical, etc. The notebook processes this data, stores it in CSV files, and builds a prediction model using polynomial regression.

### Features:
- Fetch rating data for any Lichess user.
- Supports multiple rating formats (Bullet, Blitz, Classical, etc.).
- Uses the Lichess API to retrieve rating data.
- Stores the data in CSV files for easy use and further processing.
- Predicts future ratings based on past performance using polynomial regression.

## Files

- **Lichess_Rating_Projection.ipynb:** The main Jupyter Notebook where the data is analyzed, processed, and the prediction model is built.
- Rating data CSV files: The project works with CSV files containing rating data fetched from the Lichess API. These files can contain data for any game format (e.g., Bullet, Blitz, Classical, etc.).

## Installation

To run this project, you will need the following dependencies:

- Python 3.x
- pandas
- numpy
- matplotlib
- scikit-learn
- requests (for Lichess API requests)

You can install the dependencies using the following command:
```bash
pip install -r requirements.txt
