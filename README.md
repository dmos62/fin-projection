# 💸 Personal finance projection via Monte Carlo simulation

The JupyterLite notebook:

🔗 https://dmos62.github.io/fin-projection/lab/index.html?path=worth-over-time-brownian.ipynb

---------------------------------------

## 🛠️ How to use it:

- Open the link above.

- In the top bar, click "**Run**" → "**Run All Cells**".

- Scroll down to the bottom.

- Wait ~30–60 seconds the first time (a JupyterLite notebook can be slow to start).

- You'll see sliders and a chart. Adjusting the sliders (or the number inputs) will **automatically update** the chart.

Example screenshot of what it should look like:

📷 https://i.imgur.com/sjDgZKz.png

-------------------------------

## 📈 What it does:

- Simulates the **growth of your investments over time**.
 
- Shows **percentile curves** based on Monte Carlo-style simulations:
 
  - **P50** = median outcome (most likely) 
  - **P5** and **P95** mark the pessimistic and optimistic extremes—only 5% of simulations do worse/better.

- Lets you adjust:

  - Initial investment

  - Expected return & return volatility

  - Net monthly income (positive or negative)
 
  - Expected inflation & its volatility
 
- Assumes you invest (or withdraw) your **net income monthly**.

- Uses **Geometric Brownian Motion** to run a thousand simulations that are within specified constraints and visualizes the probabilities implied by those simulations.

- The default expected return is **8%**, and volatility is **18%** — roughly in line with historical S&P 500 performance.

- Inflation is by default **3%** expected, **2%** volatility.

-------------------------

## 🧪 An experiment to try:

Set the initial investment to something like **$1 million**, and pretend you have **no income**.
Then adjust the **net monthly income (negative)** until your portfolio stays roughly flat in the **P50 (median) curve**.

In other words: what monthly withdrawal could you sustain without your portfolio shrinking in the median scenario?

Was it more or less than you expected?

---------------------------------------

## ⚠️ Caveats:

- I don’t have a finance degree — this was just a weekend project and I wouldn't be surprised if the logic is very wrong.