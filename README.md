# Bayesian-MMM

A Bayesian media mix model in PyMC. It estimates how much revenue each of 7 paid channels brings, using 104 weeks of data.

Revenue is a baseline (trend, yearly season, Cyber Week) plus the effect of each channel. Spend has a delayed effect, so I use adstock. Every channel gets its own ROAS.

What I found:
- Carry-over is short. Most of the effect comes in the week of the spend.
- Paid media drives about 39% of revenue.
- On 16 unseen weeks the error is 11.5%. A seasonal naive forecast has 24.7%.
- ch5 has the best ROI (ROAS about 1.22). ch4 is the weakest.

Files:
- `MMM_PyMC_Cagan_Deliktas.ipynb`: the full model and code
- `MMM_Report_Cagan_Deliktas.pdf`: short report with the results

The data is not in this repo.
