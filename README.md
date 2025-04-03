Derivatives Pricing with Machine Learning
Project Overview
This project focuses on using machine learning techniques to perform derivative pricing, specifically using supervised regression models to learn the Black-Scholes option pricing formula from simulated data. The Black-Scholes model is a widely used mathematical framework for pricing European options.

Black-Scholes Formula
The Black-Scholes formula used in this project is as follows:

 Stock Price:S

K: Strike Price

r: Risk-free rate

q: Annual dividend yield (set to 0 in this project)

T-t: Time to maturity

σ (sigma): Volatility

M (Moneyness): Defined as 
M
=
K
S
M= 
S
K
 

Key Features
Simulated Data Generation:

Moneyness, time to maturity, and volatility are simulated using predefined functions.

The Black-Scholes formula is applied to calculate option prices.

Machine Learning Models:

Various regression models are implemented, including Linear Regression, Decision Trees, Random Forests, Gradient Boosting, Neural Networks, and more.

Feature selection techniques are applied to identify the most impactful features.

Libraries Used:

Data manipulation: numpy, pandas

Visualization: matplotlib, seaborn

Machine learning: scikit-learn, keras

Statistical analysis: statsmodels

Time series modeling: ARIMA

Installation
To run this project, ensure you have Python installed along with the required libraries. Install dependencies using:

bash
pip install numpy pandas matplotlib seaborn scikit-learn keras statsmodels
Code Structure
True Parameters
The following parameters are defined:

python
true_alpha = 0.1
true_beta = 0.1
true_sigma0 = 0.2
risk_free_rate = 0.05
Functions for Option Pricing and Volatility
Two main functions:

option_vol_from_surface(moneyness, time_to_maturity) calculates volatility based on moneyness and time to maturity.

call_option_price(moneyness, time_to_maturity, option_vol) computes the call option price using the Black-Scholes formula.

Data Simulation
Simulated data includes:

Moneyness (
K
/
S
K/S)

Time to maturity (
T
−
t
T−t)

Volatility (
σ
σ)

Option prices

Dataset Example
Price	Moneyness	Time	Volatility
0.150	0.924	0.343	0.234
0.114	1.089	0.502	0.251
Summary Statistics
Feature	Mean	Std Dev	Min	Max
Price	0.179	0.136	0.000	0.885
Moneyness	0.997	0.251	0.117	1.918
Time	0.498	0.286	0.000	1.000
Volatility	0.256	0.030	0.200	0.363
Results and Insights
Feature importance scores from regression models indicate that:

Moneyness is the most impactful feature.

Volatility and Time to maturity also contribute significantly.

How to Run the Project
Clone the repository and navigate to the project directory.

Run the Jupyter Notebook file (Derivatives_Project.ipynb) or execute Python scripts directly.

Experiment with different regression models and analyze their performance.
