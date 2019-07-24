Portfolio Metric Testing Tool - v1.0 ReadMe

 -------The code is written on Python v.3.7.0. You would need v.3.7.x to run the code without any problems ---------

________________________________________________________________________________________________________________________________________

1. Open the file titled 'Portfolio Metric Testing Tool.ipynb' in a Jupyter notebook via Anaconda. In case you do not have Anaconda, you can download it from here: https://www.anaconda.com/distribution/
2. You can run each individual cell by hitting the 'Run' button or clicking Shift + Enter.
3. The code has two functionalities:
	a. To verify the LBO100 portfolio daily returns.
	b. To verify the LBO100 portfolio performance metrics.

Additional information is broken down below.
________________________________________________________________________________________________________________________________________

A. Verifying Daily Returns

The Daily Return part of the code uses two files as inputs - 'LBO profile - 19y.xlsm' called "Returns" henceforth and '2008_2009_constituent_aws_ranked.xlsx' called "Positions" henceforth.
The code also has an additional feature to allow the client to verify the returns for a date range or a single date.
	i. Once a date (range) is chosen, the Positions file is used to caluclate portfolio returns for the date (range). 
	ii. The portfolio return for the same date (range) is pulled from the Returns file. This was the QMIT reported portfolio return. 

Both the above values should always turn out the same. In case there are instances where the values don't match, kindly contact QuantZ capital for further clarification.

________________________________________________________________________________________________________________________________________

B. Performance Metric Calculation

The second half of the code calculates a list of metrics for the LBO100 portfolio based on the Returns file. The metrics covered by the code are:
	i. Annualized Return
	ii. Annualized Volatility
	iii. Sharpe Ratio
	iv. Sortino Ratio
	v. Maximum Drawdown
	vi. Beta to S&P
	vii. Skew
	viii. Kurtosis
_________________________________________________________________________________________________________________________________________________________________________________
