# Bitcoin Historical Data

This repository contains historical data for Bitcoin, including price, volume, and other relevant metrics. The dataset is ideal for analyzing Bitcoin's price trends, performing time-series analysis, and building predictive models.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Features](#features)
4. [How to Use](#how-to-use)
5. [Examples](#examples)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

---

## Introduction

Bitcoin is the first decentralized digital currency, and its price has been highly volatile since its inception. This repository provides historical data on Bitcoin, which can be used for various analyses, such as price prediction, trend analysis, and market behavior studies.

The dataset is updated regularly and includes key metrics such as opening price, closing price, highest price, lowest price, and trading volume.

---

## Dataset Description

The dataset contains historical Bitcoin data in CSV format. Each row represents a specific time period (e.g., daily, hourly, or minute-level data), and the columns include the following features:

- **Timestamp**: The date and time of the data point.
- **Open**: The opening price of Bitcoin for the given time period.
- **High**: The highest price of Bitcoin during the time period.
- **Low**: The lowest price of Bitcoin during the time period.
- **Close**: The closing price of Bitcoin for the time period.
- **Volume (BTC)**: The trading volume of Bitcoin during the time period.
- **Volume (Currency)**: The trading volume in the respective currency (e.g., USD).
- **Weighted Price**: The weighted price of Bitcoin for the time period.

---

## Features

- **Historical Data**: The dataset includes historical Bitcoin prices and trading volumes.
- **Multiple Timeframes**: Data is available in daily, hourly, and minute-level intervals.
- **CSV Format**: The dataset is provided in CSV format for easy integration with data analysis tools.
- **Regular Updates**: The dataset is updated regularly to include the latest Bitcoin data.

---

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/FathyHesham/Bitcoin-Historical-Data.git
   ```
2. **Navigate to the Dataset**:
   ```bash
   cd Bitcoin-Historical-Data
   ```
3. **Load the Dataset**:
   You can load the dataset using Python's `pandas` library:
   ```python
   import pandas as pd
   df = pd.read_csv('bitcoin_historical_data.csv')
   print(df.head())
   ```

---

## Examples

### Example 1: Plotting Bitcoin Price Over Time
```python
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
df = pd.read_csv('bitcoin_historical_data.csv')

# Plot the closing price over time
plt.figure(figsize=(10, 6))
plt.plot(df['Timestamp'], df['Close'], label='Bitcoin Closing Price')
plt.xlabel('Date')
plt.ylabel('Price (USD)')
plt.title('Bitcoin Price Over Time')
plt.legend()
plt.show()
```

### Example 2: Calculating Daily Returns
```python
# Calculate daily returns
df['Daily Return'] = df['Close'].pct_change()

# Plot daily returns
plt.figure(figsize=(10, 6))
plt.plot(df['Timestamp'], df['Daily Return'], label='Daily Returns', color='orange')
plt.xlabel('Date')
plt.ylabel('Daily Return')
plt.title('Bitcoin Daily Returns')
plt.legend()
plt.show()
```

---

## Contributing

Contributions are welcome! If you have suggestions for improving the dataset or adding new features, please follow these steps:

1. Fork the repository.
2. Create a new branch for your changes.
3. Submit a pull request with a detailed description of your changes.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact

For any inquiries or further information, feel free to reach out:

- **Mail**: [fathyhesham2001@gmail.com](mailto:fathyhesham2001@gmail.com)
- **LinkedIn**: [Fathy Hesham Fathy](https://www.linkedin.com/in/fathy-hesham-fathy/)

---

**Thank you for visiting the Bitcoin Historical Data repository!** 🚀
