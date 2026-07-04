# ⚽ World Cup Match Outcome Predictor

## Overview
Machine learning model predicting FIFA World Cup 2026 match 
outcomes using 154 years of international football data (1872-2026).
Achieved 56% accuracy — competitive with professional models.

## Tech Stack
Python, Pandas, Scikit-learn, Matplotlib, Seaborn

## Approach
- Filtered 49,498 matches to 19,872 competitive matches
- Built rolling team strength features (win rate, goals, form)
- Strict time-based train/test split to prevent data leakage
- Compared Logistic Regression, Random Forest, Gradient Boosting

## Results
| Model | Accuracy |
|---|---|
| Gradient Boosting | 56.08% |
| Logistic Regression | 55.75% |
| Random Forest | 53.95% |

## Key Findings
- 56% accuracy beats random guessing (33%) significantly
- Draws are hardest to predict — known challenge in football analytics
- Quality of opposition is key limitation — ELO ratings would improve this
- Home advantage measurably disappears at neutral venues

## Next Steps
- [ ] Add ELO ratings to account for opposition strength
- [ ] Build scoreline predictor
- [ ] Power BI dashboard for visualisation
- [ ] Separate knockout stage model (no draws)
