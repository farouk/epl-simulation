Licensed under the MIT License.

# EPL Title Race – Monte Carlo Simulation

This notebook simulates the remainder of an EPL season using a simple
Monte Carlo approach based on real fixtures and historical results.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/farouk/epl-simulation/blob/main/Arsenal_EPL_MonteCarlo_Colab.ipynb)
## How to run
1. Open the notebook in Colab (button above)
2. Upload your fixtures/results CSV when prompted (or set the CSV path)
3. Run all cells to reproduce the simulation + chart

## Data
Match results and fixtures are sourced from publicly available football data
(e.g. Football-Data, FBref).

The notebook expects a CSV with at least the following columns:
- HomeTeam
- AwayTeam
- FTHG (full-time home goals)
- FTAG (full-time away goals)

Played matches should have goals filled.
Remaining fixtures should have goal fields left blank (NaN).

Data files are not included to avoid redistribution issues.


## What this is
- A learning exercise in reasoning under uncertainty
- Uses goal distributions (Poisson) and actual remaining fixtures
- Simulates the rest of the season many times to estimate outcomes

## What this is NOT
- A prediction model
- A betting tool
- A fully calibrated forecasting system

## Key idea
Over a season, teams that consistently avoid bad days tend to outperform
teams that rely on occasional big wins.

## Notes
- Built in Google Colab
- Data sourced from publicly available football results
- Shared for learning and discussion

