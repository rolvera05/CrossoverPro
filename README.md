# CrossoverPro

This project showcases an elegant and efficient simple moving average (SMA) crossover strategy for trading stocks, leveraging the power of historical data. Driven by the growing demand for effective and data-driven trading strategies, this project aims to empower users to make well-informed decisions when it comes to entering and exiting positions. By harnessing the potential of reliable technical indicators, the project allows users to capitalize on market trends with greater confidence.

To facilitate a comprehensive evaluation of the strategy's performance, the project employs a range of essential metrics, including cumulative returns, Sharpe ratio, Sortino ratio, and maximum drawdown. By providing users with insightful and actionable information, this project serves as a valuable tool for traders seeking to optimize their investment strategies and stay ahead of the curve in today's dynamic financial markets.

---

## Technologies

The project is developed using Python 3 and relies on the following libraries:

* [pandas](https://github.com/google/python-fire) - For the command line interface, help page, and entrypoint.

* [numpy](https://numpy.org/install/) - Conducts a diverse range of mathematical computations on arrays.

* [plotly](https://plotly.com/python/) - A Python library that leverages the Plotly JavaScript library (plotly.js) to empower users to produce stunning interactive web-based visualizations. These visualizations can be presented within Jupyter notebooks, preserved as standalone HTML files, or integrated into purely Python-designed web applications using Dash.

* [yfinance](https://pypi.org/project/yfinance/) - API for data collection.

* [matplotlib](https://matplotlib.org/stable/users/installing/index.html) - Used to create 2D graphs and plots using python scripts.

* [seaborn](https://seaborn.pydata.org/installing.html) - Used for data science and machine learning tasks.

Ensure that you have the compatible versions of these libraries installed in your Python environment.

---

## Installation Guide

To install and run the ETF Analyzer Web Application, follow these steps:

    1. Clone the project repository from GitHub
```python
    git clone git@github.com:rolvera05/CrossoverPro.git
```
    2. Navigate to the project directory
```python
    cd CrossoverPro
```
    3. Create a virtual environment (optional but recommended)
```python
    python3 -m venv venv
```
    4. Activate the virtual environment
```python
    Windows:
    venv\Scripts\activate
    macOS/Linux:
    source venv/bin/activate
```
    5. Install the required dependencies
```python
    pip install pandas numpy plotly yfinance
```
    6. Run the web application
```python
    streamlite app.ipynb
```
    7. Open your web browser and access the application at http


---

## Usage

### Analyzing Stock Performance with SMA Crossover Strategy

1. Load the historical stock data of the desired asset.
2. Set the desired short-term and long-term moving average window periods.
3. Calculate the simple moving averages for the short-term and long-term periods.
4. Generate the buy and sell signals based on SMA crossover events.
5. Visualize the stock performance along with the buy and sell signals on an interactive plot.

### Evaluating Strategy Performance Metrics

1. Calculate the cumulative returns of the stock using the SMA crossover strategy.
2. Compute the Sharpe ratio to assess the risk-adjusted performance of the strategy.
3. Determine the Sortino ratio to evaluate the downside risk-adjusted performance.
4. Measure the maximum drawdown to understand the strategy's potential peak-to-trough loss.
5. Review the calculated performance metrics to gauge the effectiveness of the SMA crossover strategy.

### Usage Example: Implementing and Evaluating SMA Crossover Strategy

Upon running the Python script with the appropriate stock data and SMA window periods, the following output should be generated:

1. A plot visualizing the stock performance, along with buy and sell signals based on SMA crossover events.
2. A table displaying the key performance metrics: cumulative returns, Sharpe ratio, Sortino ratio, and maximum drawdown.
 

---

Upon launching the web page via Voila the following should appear:

![SMA Crossover Visualization](images/sma-crossover.png)
![SMA Crossover Cumulative Returns](images/cumulative-returns.png)

---

## Contributors

Brought to you by Rosalinda Olvera Fernandez, Alex Valenzuela, James White, Michelle Silver, Dylan Johnston


---

## License

This project is licensed under the MIT License.






[def]: Images/web_page.mov