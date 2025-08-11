# Lichess Rating Prediction Tool

An interactive Jupyter notebook that analyzes your Lichess rating history and predicts future performance using polynomial regression models.

## Features

- **Interactive Data Fetching**: Enter your Lichess username and select rating format through user-friendly widgets
- **Automated Analysis**: Fetches rating data directly from Lichess API
- **Polynomial Regression**: Trains multiple polynomial models and selects the best performing one
- **Future Predictions**: Predict your rating at any future date
- **Target Achievement**: Estimate when you'll reach specific rating goals
- **Professional Visualizations**: Clean charts showing rating history and future projections
- **Real-time Interaction**: Interactive widgets for custom predictions

## Quick Start

### Prerequisites
- Python 3.7+
- Jupyter Notebook or JupyterLab

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/Khanna-Aman/chess-rating-prediction.git
   cd chess-rating-prediction
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter:
   ```bash
   jupyter notebook
   ```

4. Open `Lichess_Rating_Projection.ipynb`

### Usage

1. **Setup**: Run the first cell to initialize the interactive widgets
2. **Input**: Enter your Lichess username and select rating format (Bullet, Blitz, Rapid, Classical)
3. **Fetch Data**: Click "Fetch Rating Data" to download your rating history
4. **Process**: Run the data processing cell to prepare your data
5. **Train Model**: Execute the model training cell to find the best polynomial fit
6. **Visualize**: Generate charts showing your rating progression and future predictions
7. **Predict**: Use interactive widgets to:
   - Predict your rating on any future date
   - Estimate when you'll reach target ratings

## How It Works

### Data Collection
- Connects to Lichess API to fetch your complete rating history
- Supports all major time controls: Bullet, Blitz, Rapid, and Classical
- Automatically handles data formatting and chronological sorting

### Model Training
- Tests polynomial regression models of degrees 1-5
- Uses 80/20 train-test split for validation
- Selects best model based on Mean Squared Error (MSE)
- Displays performance metrics for transparency

### Prediction Engine
- **Date Prediction**: Enter a target date to see your predicted rating
- **Achievement Estimation**: Enter a target rating to see when you'll likely reach it
- **Trend Analysis**: Visualizes historical data alongside future projections

## Example Output

```
Best Polynomial Degree: 3 (MSE: 1247.52)

Current rating: 2689
Predicted rating in 6 months: 2841.83
Predicted rating in 1 year: 2977.22

Estimated date to reach 2800 rating: 15-04-2025
```

## Technical Details

### Dependencies
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computations
- **matplotlib**: Data visualization
- **scikit-learn**: Machine learning models
- **requests**: API communication
- **scipy**: Advanced mathematical functions
- **ipywidgets**: Interactive notebook widgets

### Model Selection
The tool automatically tests polynomial regression models of varying complexity and selects the one with the lowest validation error, ensuring optimal prediction accuracy while avoiding overfitting.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

This tool provides statistical predictions based on historical data. Actual rating progression depends on many factors including practice consistency, game frequency, and skill development. Use predictions as estimates, not guarantees.
