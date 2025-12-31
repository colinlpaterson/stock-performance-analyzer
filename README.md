# Stock Performance Analyzer

A Streamlit web application for analyzing and comparing stock and ETF performance with interactive visualizations.

## Features

### 📈 Historical YTD Performance
- View year-to-date (YTD) performance for any stock ticker
- Compare current year against historical years
- Available for any ticker supported by Yahoo Finance

### 📊 Multi-Ticker Comparison
- Compare YTD performance across multiple tickers simultaneously
- View last full year's performance (dashed lines) alongside current YTD
- Color-coded visualization for easy comparison
- Available for any ticker supported by Yahoo Finance

## Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup

1. Clone the repository:
```bash
git clone https://github.com/colinlpaterson/stock-performance-analyzer.git
cd stock-performance-analyzer
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Running Locally

Start the Streamlit app:
```bash
streamlit run app.py
```

The app will open in your default browser at `http://localhost:8501`

### Using the App

**Historical YTD Analysis:**
1. Navigate to the "Historical YTD" page
2. Enter a stock ticker (e.g., SPY, AAPL, MSFT)
3. Select a start year (e.g., 2004)

**Multi-Ticker Comparison:**
1. Navigate to the "Ticker Comparison" page
2. Enter multiple tickers separated by commas or use the multi-select widget
3. View comparative YTD performance and last year's full performance
4. Use the color-coded charts to identify relative performance

## Data Source

This application uses **yfinance** to fetch real-time and historical stock data from Yahoo Finance.

## Project Structure

```
stock-performance-analyzer/
├── app.py                      # Main Streamlit application
├── pages/
│   ├── 1_📈_Historical_YTD.py   # Historical YTD comparison page
│   └── 2_📊_Ticker_Comparison.py # Multi-ticker comparison page
├── utils/
│   ├── __init__.py
│   ├── data_fetcher.py         # Data retrieval functions
│   └── chart_builder.py        # Plotting and visualization functions
├── requirements.txt            # Python dependencies
├── .gitignore                 # Git ignore file
└── README.md                  # This file
```

## Technologies Used

- **Streamlit**: Web application framework
- **yfinance**: Stock data retrieval
- **Plotly**: Interactive charting
- **Pandas**: Data manipulation
- **NumPy**: Numerical computations

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

## Contact

Colin Paterson - [GitHub Profile](https://github.com/colinlpaterson)

## Acknowledgments

- Data provided by Yahoo Finance via yfinance
- Built with Streamlit

---

**Note**: This application is for educational and informational purposes only. It is not financial advice. Always consult with a qualified financial advisor before making investment decisions.