# *challenge-05-042023*
---
** Repository for challenge 5 for FinTech BootCamp**
---
## Financial Planning with API's and Simulations
![Image used from original FinTech challenge files](/Starter_Code/Images/5-4-challenge-image.png)
The purpse of this challenge was to analyze a credit union member's savings and project when the member might be able to retire based on the rate of returns of the member's portfolio, where the member's portfolio comprises of stocks/bonds, and crypto currency. 

## Technologies

This project leverages python 3.7 specifically and assumes that jupyter lab has been installed. In addition, this project assumes that you the monte carlo module MCForecastTools.py in the root directory. In additon, you would need to have the following modules installed:
* json
* Alpaca
* pandas

## Resources
* Data provided by Columbia FinTech program.
* MC Simulation module provided by Columbia FinTech program

## Contributions 

Historical data and challenge questions provided by Columbia FinTech progam.
Analysis, code, and conclusions completed by Sean Senhouse

## Installation Guide
### To review challenge 5:

* First initialze the dev environment and the Jupyter lab by typing the following at the command prompt:  

```python
str("conda activate dev")
str("jupyter lab")
```
* Open the Jupter Notebook titled: **financial_planning_tools.ipynb** 

* Run all of the code

## Usage
Once the book is opened, the book is broken up two sections:
* Part 1: A financial planner for emergencies. The members will be able to use this tool to visualize their current savings. The members can then determine if they have enough reserves for an emergency fund.

* Part 2: A financial planner for retirement. This tool will forecast the performance of their retirement portfolio in 30 years. To do this, the tool will make an Alpaca API call via the Alpaca SDK to get historical price data for use in Monte Carlo simulations.

Part 1 Results: The code calculates the member's current portfolio's value. The report then tests whether the memember's savings is sufficient to replace the member's monthly income for 3 months

Figure I below shows the mix of the member's portfoilio
![Member's portfolio of stocks and bonds](/Starter_Code/Images/members_portfolio.png)


Part 2 Results: The code uses a monte carlo simulation to project the portfolio returns for 30yrs and 10 yrs. At the end of the simulation the program shows that the member will not have sufficient funds within 10yrs to retire. The report also shows the confidence 95% confidence intervals for the portfolio returns for both simulations.  

Figure I shows the 30yr returns simulation

![MC 10yr simulation plot](/Starter_Code/Images/MC_thirtyyear_sim_plot.png)

Figure II shows the 30yr returns distribution and 95% confidence intervals

![MC 10yr distribution plot](/Starter_Code/Images/MC_thirtyyear_dist_plot.png)

Figure III shows the 10yr returns simulation

![MC 30yr simulation plot](/Starter_Code/Images/MC_tenyear_sim_plot.png)

Figure IV shows the 10yr returns distribution

![MC 30yr distribution plot](/Starter_Code/Images/MC_tenyear_dist_plot.png)