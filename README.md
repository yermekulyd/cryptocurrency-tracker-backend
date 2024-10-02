# Cryptocurrency Tracker Backend

This project is a FastAPI backend that integrates with the CoinMarketCap API to retrieve cryptocurrency data such as current prices and market capitalization. The backend supports asynchronous operations, data caching, and CORS for frontend interaction

## Features

- Work with external APIs (CoinMarketCap)
- Asynchronous operations using `aiohttp`
- Data caching with `async_lru`
- CORS enabled for frontend communication

# Setup and Installation

## Prerequisites:

- Python 3.10+
- [CoinMarketCap API key](https://pro.coinmarketcap.com/)

## Steps:

1. Clone the repository:
```
git clone <repository-url>
cd <repository-directory>
```
2. Create and activate a virtual environment:
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. Install dependencies:
```
pip install -r requirements.txt
```
4. Create a `.env` file in the root directory and add your CoinMarketCap API key:
```
CMC_API_KEY=your_coinmarketcap_api_key
```
5. Run the FastAPI application:
```
uvicorn src.main:app --reload
```
6. Access the API documentation via Swagger UI at `http://127.0.0.1:8000/docs`

