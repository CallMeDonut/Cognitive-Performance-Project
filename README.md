# Cognitive Human Performance Prediction


## Objective

To build a predictive model that estimates cognitive performance (Cognitive_Score) based solely on real-life, modifiable lifestyle and behavioral indicators.

## Dataset Overview

Original dataset includes cognitive scores and various behavioral/lifestyle features.

AI-derived fields (e.g., ai_score) were removed to avoid data leakage.

Only features reflecting user habits, behaviors, or health metrics were retained.

## Model Performance Summary

Model: R², RMSE

Linear Regression: 0.9956, 1.5210

Random Forest: 0.9879, 2.5232

Linear model nearly matches Random Forest performance, suggesting mostly linear relationships.

Strong predictive power confirms the relevance of selected behavioral features.

## Top Predictive Features

These were identified via Random Forest feature importances:

Sleep Hours — Strong positive correlation; more sleep = better cognitive performance.

Physical Activity — Exercise boosts memory and executive function.

Screen Time — Negatively associated; may impair focus or sleep.

Hydration Level — Important for cognitive processing speed.

Stress Score — Higher stress = lower scores.

Learning Hours — Time spent reading or learning improves scores.

## Key Insights

Behavioral factors alone can nearly perfectly predict cognitive score.

The model is not overfitting: shuffled target test yielded R² near zero, indicating real signal.

Consistent, positive behavioral changes (e.g., more sleep, less screen time) can lead to measurable cognitive improvements.

The model could be used to simulate interventions or generate personalized habit recommendations.

## Recommendations

Deploy as an interactive app to let users input behaviors and see predicted cognition.

Incorporate SHAP or LIME to visually explain individual predictions.

Explore longitudinal use: can changes in behavior over time predict cognitive trajectory?

Expand features: consider adding nutrition, social interaction, and mood scores.

## Conclusion

This project demonstrates the feasibility of accurately modeling cognitive performance based on lifestyle data. It provides a foundation for real-world tools that empower users to enhance mental performance through measurable, actionable behaviors.
