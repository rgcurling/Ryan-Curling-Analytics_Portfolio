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

- Statistical Modeling: Mastery of MLE and MoM for parameter estimation.
  
- R Programming: Writing custom PDF/PMF functions, applying the fitdist package for parameter estimation, and creating visualizations such as histograms and density plots.
  
- Mathematical Analysis: Simplifying likelihood functions and deriving parameter estimators.
  
- Data Visualization: Using plots to evaluate model fits and interpret statistical results.

Technology: R, itdistrplus for parameter estimation, and data visualization tools for plotting histograms and density curves. Wolfram Alpha for solving equations and verifying mathematical derivations. RData files for reproducible analysis of datasets.

Conclusion:

- Jackson Distribution: Demonstrated its ability to model skewed-right data with possible negative values, relevant for scenarios such as modeling account balances.

- Lomax Distribution: Applied to heavy-tailed data, useful in economics, actuarial science, and business analytics.

- Cannon Distribution: Explored for its U-shaped failure rates, effectively modeling product lifespans where early and late failures are more likely.

- Zero-Truncated Binomial: Modeled counts where zero is not a valid outcome, such as coupon usage among active customers.

- Model Evaluation: AIC comparisons provided insights into the trade-offs between model simplicity and fit accuracy.
  
- Visualization: Overlaid histograms with fitted density curves highlighted the quality of the fits.

The project reinforced the value of probabilistic modeling in analyzing real-world datasets. By combining R programming, mathematical derivations, and statistical tools, the work showcased the importance of selecting and validating appropriate probability distributions for accurate data representation and decision-making in practical applications.


## Monte Carlo Simulations 


Goal: This assignment aimed to help me deepen my understanding of Monte Carlo simulations and how they can be used to estimate probabilities and solve real-world problems involving randomness and uncertainty.

Description: In this project, I applied Monte Carlo simulation techniques to tackle various scenarios, including candy consumption patterns, call center operations, inspection processes, restaurant revenue simulations, stock price changes, and even baseball inning simulations. I wrote R code to model these situations, estimate probabilities, and analyze outcomes. Each problem required thoughtful implementation and interpretation of the results, providing hands-on experience with computational simulations.

Skills I Gained: 

- Monte Carlo Simulation: Learned how to design and implement simulations to model random events.
  
- R Programming: Improved my ability to write efficient code for sampling, looping, and analyzing simulated data.
  
- Statistical Estimation: Gained experience estimating probabilities, means, and distributions for complex processes.
  
- Data Visualization: Developed histograms and plots to visualize and interpret simulated data distributions.
  
Tools and Techniques:

- R Functions: Used sample(), cumsum(), and logical operators to implement simulations and analyze results.
  
- Custom Probability Models: Created tailored simulations for specific scenarios, such as weighted sampling and conditional probabilities.
  
- Visualization: Plotted histograms and data trends to evaluate distributions and outcomes.
  
Conclusion: 

- Candy Consumption: Estimated that 42% of scenarios resulted in 25 kids taking 40 or more candies, and 3.9% of cases allowed 90 kids to take candy from a bowl of 120 pieces.
- Call Center Operations: Simulated daily call volumes and found that exceeding 2,500 calls in February had a 10% chance.
- Inspection Processes: Determined that parts inspected exactly 12 times occurred only 0.5% of the time, while 56.2% of scenarios had more parts inspected 7 times than 10 times.
- Restaurant Simulation: Simulated nightly revenue and found a 7.6% chance of earning less than $400, with revenue distributions closely reflecting real-world variability.
- Stock Price Evolution: Simulated 100-day stock price changes and calculated a 14% chance of prices remaining in the desired range of $75–$95.
- Candy Pack Analysis: Found that in 22% of scenarios, pink candies were not the most frequent color in a pack of 30. I also explored how this probability changes with different pack sizes.

This project gave me a deeper appreciation for the versatility of Monte Carlo simulations in addressing real-world problems. By creating and running simulations, I gained hands-on experience in modeling randomness and analyzing complex systems. I also sharpened my R programming skills and learned how to visualize and interpret simulation results effectively. The results from each scenario demonstrated the power of probabilistic thinking in making data-driven decisions and understanding stochastic processes.

## Comparing Averages and Bootstrapping 

Goal: To analyze statistical differences between groups and apply bootstrapping techniques to estimate confidence intervals for various parameters, enhancing the ability to make data-driven decisions.

Description: This project focuses on comparing group averages, assessing statistical significance, and using bootstrapping to estimate confidence intervals for non-standard scenarios. Datasets include movie performance indicators, food ratings, product return rates, and NBA player statistics. Tasks involved implementing hypothesis tests, computing effect sizes, creating connecting letters reports, and programming bootstrap simulations in R.

Skills:

- Hypothesis Testing: Determining statistical significance of differences between groups (e.g., t-tests, ANOVA).
  
- Effect Size Measurement: Calculating Cohen’s d and interpreting the practical significance of differences.
  
- Bootstrapping: Implementing resampling methods to estimate confidence intervals for medians, correlations, and percentiles.
  
- Data Visualization: Using histograms, boxplots, and connecting letters reports to interpret results.
  
Technology:

- R Packages: boot for bootstrap confidence intervals, multcomp for multiple comparisons, and visualization tools.
  
- Statistical Models: Linear regression and correlation analysis for evaluating relationships between variables.
  
- Custom Implementations: For-loop programming for percentile bootstraps and manual confidence interval estimation.
  
Results:

- Drivers of Movie Success:
    - ROI and Audience Ratings: Movies in cinematic universes had significantly higher ROI (+0.47 vs. -0.25; large effect size) and slightly          higher audience ratings (+0.68 vs. 0.66; small effect size).
    - Runtime Impact: Audience ratings increased with runtime, with movies over 130 minutes receiving the highest scores.
      
- Food Ratings:
  - No significant difference was found between recipes when using the correct test, as the confidence interval for the difference in ratings       contained zero.
    
- Product Return Rates:
    - Statistically significant differences in return rates between some groups were identified, while others were "statistically tied."
    - Connecting letters reports clarified which product categories were distinct in return rates.
      
- NBA Player Statistics:
    - Bootstrapped 95% confidence intervals confirmed:
    - Median points scored per game ranged from 6.8 to 7.4, making 7.3 a plausible value.
    - True correlation between height and rebounds was between 0.42 and 0.48.
    - The 75th percentile of shooting efficiency ranged from 0.588 to 0.595.
      
Conclusion: 

This project demonstrated the importance of rigorous statistical analysis and bootstrapping in understanding data. By combining traditional hypothesis testing with resampling methods, I gained insights into differences between groups and uncertainty in parameter estimates. These techniques are critical for analyzing real-world datasets and providing actionable recommendations.














