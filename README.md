# **Team 5 - Do Moving Average Crossover Trading Strategies Really Work?**

### Team members
Hanna Ho, Claudia Martinez, Atousa Mirzaei-Rezaei, Jalal Huseynov

## **Project description**

Moving Average (MA) Crossover Strategy is very well known and the most simple long-only trading strategy. Signals to buy is depending on the crossover of short lookback period over long lookback period. In contrast, the sell signal is triggered when MA long lookback crosses the MA short lookback.Our goal is to examine whether MA crossover strategies benefit for S&P ETF investors from both return and risk perspective. In this project, we will test four popular strategies which are 50 SMA crossing 200 SMA ,50 SMA crossing 100 SMA ,20 EMA crossing 50 SMA, and 11 EMA crossing the 49 EMA. 

## **Dataset that was used**
We used Pandas Datareader to get "SPY" data from yfinance (Yahoo). Even though we did not cover this in the class, we found it easy to use. After we checked the data, we saw that data is clean and it does not any cleaning.

---

`from pandas_datareader import data `
 
`import yfinance as yf`

---

`yf.Tickers(tickers)`

`panel_data = yf.download(tickers, start = start_date, end = end_date, interval = interval)`

---

## **Coding process**

    Our coding process happened in this flow:
    - Import Libraries
    - Declare variables
    - Import "SPY" ETF data
    - Check/Clean data
    - Calculate the benchmark results for our choosen ETF, "SPY"
    - Calculate the results for each strategy
    - Plot findings
    - Build dashboard for findings

## **Findings**

**Strategy 1 : 50 SMA crossing 200 SMA**


![alt text](https://github.com/brilliantlyc/Project-1/blob/main/strategy1_vs_bm_cumulative_return.png "strategy1_vs_bm_cumulative_return")

Above chart shows strategy 1's total return vs SPY total return.

![alt text](https://github.com/brilliantlyc/Project-1/blob/main/strategy1_drawdown_pct.png "strategy1_drawdown")


**Strategy 2 : 50 SMA crossing 100 SMA**

![alt text](https://github.com/brilliantlyc/Project-1/blob/main/strategy2_vs_bm_cumulative_return.png "strategy2_vs_bm_cumulative_return")

Above chart shows strategy 2's total return vs SPY total return.

![alt text](https://github.com/brilliantlyc/Project-1/blob/main/strategy2_drawdown_pct.png "strategy2_drawdown")


**Strategy 3 : 20 EMA crossing 50 SMA**

![alt text](https://github.com/brilliantlyc/Project-1/blob/main/strategy3_vs_bm_cumulative_return.png "strategy3_vs_bm_cumulative_return")

Above chart shows strategy 3's total return vs SPY total return.

![alt text](https://github.com/brilliantlyc/Project-1/blob/main/strategy3_drawdown_pct.png "strategy3_drawdown")


**Strategy 4 : 11 EMA crossing the 49 EMA**

![alt text](https://github.com/brilliantlyc/Project-1/blob/main/strategy4_vs_bm_cumulative_return.png "strategy4_vs_bm_cumulative_return")

Above chart shows strategy 4's total return vs SPY total return.

![alt text](https://github.com/brilliantlyc/Project-1/blob/main/strategy4_drawdown_pct.png "strategy4_drawdown")


**Comparision of strategy returns**

![alt text](https://github.com/brilliantlyc/Project-1/blob/main/comparison_cumulative_returns.png "Comparision of strategy returns")

Above chart shows all the strategy returns.

## **If we had more time...**

If we had more time, first thing we would do to perfect the code. This includes writing functions that can be implemented with various strategies. We would also love to calculate new performance indicators and use them to compare the performance of each strategy. In addition, we could test the peformance of other trading indicators including RSI, MACD.