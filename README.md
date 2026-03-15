# D1 Softball Early-Season Volatility Tracker (2026)

Interactive analytics dashboard identifying **inflated records, hidden contenders, and volatility profiles** in NCAA Division I Softball.

🔗 [Live Dashboard](https://kbsmd-sportsmusicdata.github.io/softball-fraud-check-pages/)

This project evaluates whether a team's record aligns with its underlying performance using **Pythagorean expectation, strength of schedule, and team strength metrics**.

The tool highlights:

- Teams outperforming their run differential ("running hot")  
- Teams underperforming their metrics ("quiet risers")  
- Teams whose records are validated by strong competition  

It functions as a **decision-support system for coaching preparation, opponent scouting, and tournament projection**.

---

# Dashboard Preview

![Softball Volatility Dashboard](dashboard-preview.png)

---

# Dataset Scope

The dashboard analyzes NCAA Division I Softball performance during the **early 2026 season** using aggregated team-level metrics.

Key dataset characteristics:

- Division I teams analyzed  
- Early-season performance window  
- Run differential based metrics  
- Strength-of-schedule adjustments  

The goal is to identify **structural strength vs short-term variance** early in the season.

---

# How the Model Works

The volatility model evaluates teams using three primary indicators.

### Fraud Delta

Fraud Delta = Actual Win% − Pythagorean Win%

Measures how far a team's record deviates from what its run differential predicts.

- Positive values indicate **overperformance** relative to underlying run profile.
- Negative values indicate **underperformance** that may correct over time.

---

### Strength of Schedule (SOS)

Measures opponent quality faced.

- This prevents inflated records built on weak competition from appearing stronger than they are.

---

### Team Strength Rating (TSR)

Composite metric synthesizing:

- offensive production  
- pitching strength
- schedule context  

Used to identify **structural team quality independent of record**.

---

# Volatility Tiers

Teams are classified into three volatility profiles.

## 📉 Regression Candidates (Overperforming + Weak SOS) **Overperforming record + weak schedule**

Indicators:

- High Fraud Delta  
- Below-average SOS  

Implications:

- Likely cooling once conference play begins  
- Record may not reflect sustainable run profile  
- Pressure situations may expose bullpen depth  

---

## 📈 Late-Season Risers

**Strong metrics but underperforming record**

Indicators:

- Negative Fraud Delta  
- Strong TSR  

Implications:

- Strong buy-low scouting targets  
- Underestimated by rankings  
- Likely positive regression as variance stabilizes  

---

## 🏆 True Contenders **Record validated by underlying metrics + High SOS**

Indicators:

- Balanced Fraud Delta  
- High SOS  

Implications:

- Performance supported by quality competition  
- Lower variance risk  
- Reliable postseason profile  

---

# 🎯 Coaching Implications

This dashboard is designed as a **coaching intelligence tool**.

Potential uses include:

### Scouting Preparation

Identify opponents with inflated records vs genuine strength.

---

### Game Planning

Adjust strategy against:

- high killshot teams  
- variance-driven opponents  
- schedule-inflated programs  

---

### Tournament Projection

Evaluate which teams are likely to:

- regress  
- surge late season  
- sustain current performance levels  

---

# 📅 Weekly Use Examples

### Monday Review

Refresh volatility tiers and identify tier shifts.

Examples:

- Stable → Overperforming  
- Underperforming → Contender  

---

### Midweek Opponent Prep

Evaluate upcoming opponents using:

- Fraud Tier  
- SOS  
- TSR  

---

### Series Planning

Stress-test teams currently **running hot**.

Adjust bullpen usage expectations and leverage situations.

---

### Selection Season

Compare résumé strength vs structural strength.

Identify potential **over-seeded or under-seeded teams**.

---

# Key Metrics Reference

### Pythagorean Expectation

Expected win percentage derived from runs scored and runs allowed.

PYTHAG = RF² / (RF² + RA²)

---

### Fraud Delta

Difference between actual win percentage and Pythagorean expectation.

Positive = overperformance  
Negative = underperformance

---

### Killshot Ratio

Measures game-changing scoring bursts: An inning where a team scores **2+ runs while allowing zero**.

Used to evaluate **high-leverage offensive volatility**.

---

# Repository Structure

```
softball-fraud-check-pages
│
├── index.html # Interactive volatility dashboard
├── README.md # Project documentation
├── dashboard-preview.png # Screenshot used in README
│
└── data
  └── processed_metrics.csv
```

---

# Tech Stack

- Python — data cleaning and metric calculation  
- HTML / CSS / JavaScript — dashboard interface  
- GitHub Pages — public dashboard hosting  

---

# Portfolio Context

This project is part of a broader [sports analytics portfolio](https://www.notion.so/krystal-beasley/Sports-Analyst-Portfolio-231077fe20b880b381b7f9877bee2021) focused on:

- performance diagnostics  
- coaching decision-support tools  
- predictive and volatility modeling in women's sports  

Related work includes NCAA coaching pipeline research and demographic analytics dashboards.

---

# Author

**Krystal Beasley**  
Sports Analytics Portfolio

[LinkedIn](https://www.linkedin.com/in/krystalbeasley/) | [GitHub](https://github.com/kbsmd-sportsmusicdata)

Email Me: hey@krystalbcreative.com
