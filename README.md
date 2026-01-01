# Linear-Reg-Fails
This repository contains the Python implementation for my Medium article on Anscombe’s Quartet. It demonstrates why summary statistics (mean, variance, correlation) are not enough to understand a dataset and why data visualization is a mandatory step in Linear Regression
# The Problem? 
Can four datasets with identical statistical properties look completely different?
Mean of x: 9.0
Mean of y: 7.50
Correlation: 0.816
Regression Line: y = 3 + 0.5x
Mathematically, they are clones. Visually, they are worlds apart.
# Implementation :-
The code  uses:Pandas: For data manipulation. Seaborn: To load the built-in dataset and perform advanced plotting. Matplotlib: For plot customization and rendering.The "Blind" SummaryWe calculate the descriptive statistics for all four datasets to show how they trick a standard Linear Regression model.The Visual RevealWe use sns.lmplot() to plot the four datasets side-by-side, revealing:Dataset I: A standard linear relationship.Dataset II: A non-linear (parabolic) relationship.Dataset III: A linear relationship broken by a high-leverage outlier.Dataset IV: A vertical cluster that incorrectly suggests a trend due to a single outlier.
