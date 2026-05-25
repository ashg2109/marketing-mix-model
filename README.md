# Marketing Mix Model (MMM)
### OLS Regression with Adstock Effects - Budget Optimisation Analysis

## Overview
Built a Marketing Mix Model using R to measure the ROI of 4 marketing 
channels (TV, Digital, Email, Search) across 3 years of weekly data, 
and identified an optimal budget reallocation strategy.

## Key Results
| Metric | Value |
|---|---|
| Model R-squared | 0.714 |
| Data | 156 weeks (3 years) |
| Channels analysed | TV · Digital · Email · Search |
| Annual sales lift (optimised budget) | **+$439,100** |

## Channel ROI ($ sales per $1,000 spent)
| Channel | ROI | Budget Share | Verdict |
|---|---|---|---|
| Email | $1,896 | 7% | Underinvested ✅ |
| Search | $1,623 | 15% | Increase spend |
| Digital | $1,006 | 21% | Maintain |
| TV | $595 | 57% | Overinvested ⚠️ |

## Recommendation
Shift 20% of TV budget to Email (+30%), Digital (+15%), and Search (+10%).

**Projected impact: +$439,100 in annual sales with no increase in total budget.**

## Methodology
- Adstock transformation to model advertising carryover effects
- OLS multiple regression (all channels significant at p < 0.001)
- Sales contribution decomposition by channel
- Budget scenario analysis - what-if modelling

## Tech Stack
R · tidyverse · ggplot2 · broom · OLS Regression · Adstock Modelling

## Files
- `mmm_analysis.R` - full R script
- `marketing_data.csv` - simulated weekly marketing dataset
- `sales_trend.png` - 3-year sales trend
- `spend_vs_sales.png` - channel spend vs sales correlation
- `contribution_chart.png` - sales decomposition by component
- `mmm_final_data.csv` - final processed dataset
