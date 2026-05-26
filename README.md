# Does Outside Money Win Elections?
### Analyzing Super PAC Spending and Electoral Outcomes in 2024 U.S. House Races

## Overview
This project examines whether Super PAC independent expenditures are associated with better electoral outcomes in 2024 U.S. House races. We combine three public datasets to analyze spending patterns, partisan differences, and predictive power of outside money across competitive and safe congressional districts.

## Research Questions
1. Is Super PAC spending associated with electoral outcomes (vote share and win/loss)?
2. Is Super PAC spending more important than a candidate's own fundraising?
3. Where does Super PAC money flow — competitive or safe districts?
4. Are there partisan differences in how Super PAC money is deployed?

## Data Sources
| Dataset | Source | Description |
|---------|--------|-------------|
| U.S. House Election Results 1976–2024 | MIT Election Lab / Harvard Dataverse | District-level vote shares and margins |
| FEC Independent Expenditures | FEC.gov (itpas2.txt) | Committee-level spending FOR and AGAINST candidates |
| FEC Candidate Summary | FEC.gov (weball24.txt) | Total disbursements and incumbency status |

## Key Findings
- Toss-up districts receive 5× more Super PAC spending than Safe districts on average
- Candidates with Super PAC support win 55% of races vs 41% without — a 14 percentage point gap
- After controlling for party and incumbency, Super PAC spending is a weaker predictor than structural factors
- Democrats receive more absolute Super PAC dollars; Republicans show higher relative dependence on outside money
- Incumbents win 81% of races regardless of spending level

## Methods
- SQL (SQLite): 10 queries including JOINs, window functions, and subqueries
- Python: EDA with matplotlib visualizations, linear and logistic regression models
- Feature engineering: log transformations, dummy variables, incumbency merge, district competitiveness classification
- Models: Linear Regression (R² = 0.143) and Logistic Regression (Accuracy = 67%)

## Files
1) Main_Notebook.ipynb        # Full analysis with narrative
2)SQL_Queries_SuperPAC.ipynb # Standalone SQL queries file
3)SuperPAC_Presentation.pptx # Presentation slides
4) README.md

## Tools
Python · SQL · SQLite · pandas · matplotlib · scikit-learn · Tableau
