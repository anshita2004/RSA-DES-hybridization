
# RSA-AES Hybrid Encryption & Machine Learning Model

This project demonstrates a hybrid cryptography system that combines RSA and AES encryption for secure data processing and applies machine learning techniques to model encryption time based on various parameters.

## Features

- **AES Encryption** for data confidentiality.
- **RSA Encryption** for secure key exchange.
- **Hybrid Encryption** combining AES & RSA.
- **Machine Learning** model using Random Forest Regressor to predict encryption time.
- **Data Integrity Check** using SHA-256 hashing.
- **Data Visualization** with matplotlib and seaborn.

## Requirements

- Python 3.7+
- pandas
- numpy
- cryptography
- matplotlib
- seaborn
- plotly
- scikit-learn
- pycryptodome

## Installation

Install the required dependencies using pip:

```bash
pip install pandas numpy cryptography matplotlib seaborn plotly scikit-learn pycryptodome
```

## File Structure

- `cryptography_model.py` – Main script combining encryption, decryption, integrity verification, and ML model training.

## Modules Overview

### 1. Dataset Creation

Creates a synthetic dataset of various encryption algorithms and parameters such as block size, key size, encryption/decryption times, and memory usage.

### 2. Encryption & Decryption

Uses the `cryptography` package to encrypt and decrypt algorithm names using Fernet (AES).

### 3. Machine Learning Model

Trains a `RandomForestRegressor` to predict encryption time based on algorithm characteristics.

### 4. Data Integrity

Uses SHA-256 hashing to verify the integrity of the encrypted dataset.

### 5. Hybrid Encryption (RSA + AES)

Implements hybrid encryption to secure sample data using AES keys encrypted with RSA public keys.

### 6. Simulation & ML Prediction

Simulates encryption on different file sizes and types, collecting performance data, and fits an ML model to predict encryption time.

## Running the Script

To run the full simulation and model:

```bash
python cryptography_model.py
```

## Output

- Model performance metrics: MSE, R² score
- Scatter plot comparing actual vs predicted encryption times

## License

This project is provided for academic and research purposes only.
