# 🏠 House Price ML Pipeline

A simple machine learning pipeline to predict house prices. This project includes data ingestion, preprocessing, model training, evaluation, and a FastAPI-based deployment.

## 📁 Structure
- `data/`: Raw and processed CSV files
- `src/`: Modular code (ingest, preprocess, train, evaluate, serve)
- `models/`: Saved model files
- `scripts/`: One-click pipeline runner
- `notebooks/`: EDA and experiments

## 🚀 Quick Start

```bash
# Clone and setup
git clone https://github.com/yourusername/house-price-ml-pipeline.git
cd house-price-ml-pipeline
pip install -r requirements.txt

# Run the pipeline
python scripts/pipeline.py

# Serve the model
uvicorn src.serve.app:app --reload
```

## 🔮 API Endpoint
After running the server, visit: [http://localhost:8000/docs](http://localhost:8000/docs)

## 📦 Sample Input

```json
{
  "sqft_living": 2000,
  "bedrooms": 3,
  "bathrooms": 2
}
```

## ✅ Sample Output

```json
{
  "predicted_price": 450000.0
}
```

