This is a retirement corpus withdrawal simulator which is useful for anyone who wants to see what should be the best strategy to withdraw some amount monthly from an intial corpus. 
It basically computes failure probability at the end of a certain time peroid (say 30 years) for any strategy where failure means running out of money before the end of that time period.
It takes into account past returns of Nifty50 and historical inflation rates to simulate a possible future of say 30 years and runs simulation of the strategy. 
Multiple such futures are randomly sampled to finally compute the failure probability.
This technique is much more realistic than usual SWP calculators which assume a fixed rate of returns.

Currently 3 different strategies are includes:
1. Pure equity strategy
2. Equity-Debt hybrid strategy
3. A strategy where withdrawal is purely made from debt part of the corpus for M months (say 100 months) and at the end of M months the amount equal to next 100 months of spend is transfered from equity to debt.

User inputs needed:
Y = 30 #No. of years to simulate
W = 3.5 #Withdrawal rate
DR_diff = 1.0 #Debt returns differential with current inflation

IC = 20000000 # Initial Corpus
M = 100 # No. of months in a cycle of equity-debt shuffling (needed in the 3rd strategy)
Debt_ratio = 0.4 # Fraction of initial corpus in debt (needed in the 2nd strategy)
Rb_M = 12 # No. of months to check and re-balance debt/equity ratio to Debt_ratio (needed in the 2nd strategy)

If interested to know more or to collaborate, please connect on schnpwr@gmail.com
