# Mini Capstone: Crypto Whale & Price Data Pipeline

This project builds a data pipeline for fetching, merging, and visualizing cryptocurrency price and whale transaction data. It uses Python, Jupyter Notebooks, and APIs from CoinGecko and Dune Analytics.

## Project Structure

- **minic/Notebooks/**
  - `01_fetch_price_data.ipynb`  
    Fetches historical price data for Dogwifcoin ($WIF) from the CoinGecko API and saves it as a pandas DataFrame.
  - `02_fetch_whale_data.ipynb`  
    Retrieves whale transaction counts from Dune Analytics and saves the results.
  - `03_merge_and_analyze.ipynb`  
    Merges price and whale data, aligns timestamps, and prepares the dataset for analysis.
  - `04_visualize.ipynb`  
    Visualizes the relationship between whale activity and price changes using matplotlib.

- **minic/Database/**  
  Stores processed data files (e.g., `prices_wif.joblib`, `whales_wif.joblib`, `merged_wif_data.joblib`).

- **minic/.env**  
  Stores API keys for CoinGecko and Dune Analytics (not tracked by git).

## Setup Instructions

1. **Clone the repository**  
   Download or clone this project to your local machine.

2. **Install dependencies**  
   Install required Python packages:
   ```bash
   pip install pandas requests joblib python-dotenv matplotlib
   ```

3. **API Key Setup**  
   - Register for CoinGecko and Dune Analytics API keys.
   - Create a `.env` file in `minic/`:
     ```
     GECKO_API_KEY=your_coingecko_api_key
     DUNE_API_KEY=your_dune_api_key
     ```

4. **Run Notebooks**  
   Open the notebooks in Jupyter or VS Code and run each step in order.

## Usage

- Fetch and store price and whale transaction data.
- Merge and align datasets for analysis.
- Visualize trends and relationships between whale activity and price.

## License

This project is for educational purposes and is licensed under the MIT License. See `LICENSE` for details.