# Data Analysis in R

## Probability Models for Continuous Quantites

Goal: To create probability models for continuous quantities in various business cases.

Description: This project explores probability models for continuous data, using R to analyze PDFs, CDFs, and descriptive statistics. It involves fitting real-world data (e.g., MLB stats, Spotify features) to distributions like normal, Weibull, and beta, evaluating their fit with statistical measures and visualizations.

Skills: R, probability modeling, data visualization, distribution fitting, descriptive statistics, integration, optimization, real-world data analysis, statistical interpretation, predictive modeling.

Technology: R, ggplot2, fitdistrplus.

Results: The results demonstrated that different distributions (e.g., Weibull, beta) are best suited for modeling specific data characteristics, as seen in MLB stats and Spotify features. We learned how to assess distribution fits using statistical metrics (AIC) and visual tools (QQ plots, histograms), highlighting the importance of selecting appropriate models for accurate data representation and interpretation. This analysis reinforced the utility of probabilistic modeling in real-world applications.

## Estimating Parameters in Probability Distributions

Goal: To master parameter estimation techniques for custom probability distributions using Maximum Likelihood Estimation (MLE) and Method of Moments (MoM). The assignment emphasizes fitting specialized distributions to real-world datasets, comparing model fits, and visualizing results.

Description: This project involves estimating parameters for niche probability distributions, including the Jackson, Lomax, Cannon, and zero-truncated Binomial distributions. By implementing custom probability functions in R and fitting them with the fitdist package, the work explores their applications in modeling real-world data scenarios, such as checking account balances, coupon redemption rates, and product failure rates. The tasks also include comparing model performance using metrics like the Akaike Information Criterion (AIC) and validating parameter estimates through visual and statistical means.

Skills: 

Statistical Modeling: Mastery of MLE and MoM for parameter estimation.
R Programming: Writing custom PDF/PMF functions, applying the fitdist package for parameter estimation, and creating visualizations such as histograms and density plots.
Mathematical Analysis: Simplifying likelihood functions and deriving parameter estimators.
Data Visualization: Using plots to evaluate model fits and interpret statistical results.

Technology: R, itdistrplus for parameter estimation, and data visualization tools for plotting histograms and density curves. Wolfram Alpha for solving equations and verifying mathematical derivations. RData files for reproducible analysis of datasets.

Conclusion:

Jackson Distribution: Demonstrated its ability to model skewed-right data with possible negative values, relevant for scenarios such as modeling account balances.

Lomax Distribution: Applied to heavy-tailed data, useful in economics, actuarial science, and business analytics.

Cannon Distribution: Explored for its U-shaped failure rates, effectively modeling product lifespans where early and late failures are more likely.

Zero-Truncated Binomial: Modeled counts where zero is not a valid outcome, such as coupon usage among active customers.

Model Evaluation: AIC comparisons provided insights into the trade-offs between model simplicity and fit accuracy.
Visualization: Overlaid histograms with fitted density curves highlighted the quality of the fits.

The project reinforced the value of probabilistic modeling in analyzing real-world datasets. By combining R programming, mathematical derivations, and statistical tools, the work showcased the importance of selecting and validating appropriate probability distributions for accurate data representation and decision-making in practical applications.
