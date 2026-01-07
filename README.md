# EPL Title Race Simulation

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/farouk/epl-simulation/blob/main/Arsenal_EPL_MonteCarlo_Colab.ipynb)

A simple Monte Carlo simulation of the English Premier League title race built in Google Colab.

This notebook models the remainder of an EPL season using:
- real played results
- real remaining fixtures
- a Poisson goal model (home/away strengths)
- EPL tie-break rules (points → goal difference → goals scored)

It was shared as a fun exercise in reasoning under uncertainty.

---

## 📥 How to Run

1. Click the **Open in Colab** badge above  
2. Upload the required EPL results and fixtures CSVs when prompted  
3. Run all cells to reproduce the simulations and visual outputs

---

## 📊 Data Expectations

This notebook expects the following columns in your data:

| Column | Description |
|--------|-------------|
| `HomeTeam` | Home team name |
| `AwayTeam` | Away team name |
| `FTHG` | Full-time home goals (played matches) |
| `FTAG` | Full-time away goals (played matches) |

- Played matches should have goals filled
- Remaining fixtures should have goal fields blank (`NaN`) so the model simulates them

You can source match results from publicly available sites such as Football-Data or FBref.

---

## 🚫 Data Files Not Included

Data files are not included due to redistribution/licensing restrictions.  
Please source your own CSVs as described above.

---

## ❗ What This Is NOT

- not a betting model  
- not a fully calibrated prediction system  
- not guaranteed to reflect real outcomes

It’s an educational simulation that explores outcomes under uncertainty.

---

## 📄 License

This project is licensed under the **MIT License** — see the `LICENSE` file for details.
