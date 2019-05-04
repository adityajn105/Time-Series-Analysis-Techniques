# Time-Series-Analysis-Techniques

## How to get data
1. Install Quandl as `pip install quandl`
2. Use following snippet to download data:
```
import quandl
data = quandl.get("WIKI/AAPL",start_date="1990-01-01",end_date="2018-12-31",collapse="weekly")
data = data[['Adj. Open','Adj. High','Adj. Low','Adj. Close','Adj. Volume']]
data.rename(columns={'Adj. Open':'Open','Adj. High':'High','Adj. Low':'Low','Adj. Close':'Close','Adj. Volume':'Volume'},inplace=True)
data.to_csv('APPL.csv',index=True)
```

## About Stock Market Data
