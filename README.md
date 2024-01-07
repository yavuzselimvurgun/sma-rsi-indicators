## 'A package that allows you to calculate sma and rsi indicators from a given csv file and outputs the indicators to a given csv file.'

### How to Install:
```
pip install sma-rsi-indicators==0.1.5
```

### Example Usage:
```Python
import sma_rsi_indicators

csv_path = "orcl.csv" # Insert the path to your csv file here
list_of_data = sma_rsi_indicators.convert_to_dict(csv_path)

sma_rsi_indicators.calculate_sma(list_of_data,"orcl-sma.csv")
sma_rsi_indicators.calculate_rsi(list_of_data,"orcl-rsi.csv")

```
***
Your csv file should contain columns called "Date" and "Close" indicating the dates and the closing values of those dates for this module to work.

The calculate_sma method calculates Simple Moving Averages for a 5-day window.

The calculate_rsi method calculates Relative Strength Indices for a 14-day window.

PyPI: [sma_rsi_indicators](https://pypi.org/project/sma-rsi-indicators/)
