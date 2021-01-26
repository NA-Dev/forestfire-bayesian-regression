# Forest Fire Bayesian Regression



This project uses PyMC3 to calculate two Bayesian Regression Models given data on forest weather and moisture conditions -- one logistic model for whether a forest fire will occur, and one linear model for burn area 

PyMCS uses Markov Chain Monte Carlo (MCMC) and Variational Inference (VI) to approximate the statistical distribution of each feature for the population from which the data has likely been drawn. These distributions can be inspected to get an idea of how much uncertainty and variation there is in the model.

The most predictive features are wind, temperature, rain, and humidity. Results show that the burn area model has less uncertainty than the occurrence model, but unfortunately both had high uncertainty. It seems that these indicators can only give a general idea of risk level.

To improve the models, there are a few ideas. First additional data be collected to include firefighter availability. Second, data could be added on geographic location so a hierarchical model could be attempted. Second, adding timestamps for each data row could enable time-series analysis (lag) to account for days when risk has been elevated for extended periods of time.



Final report: https://github.com/NA-Dev/forestfire-bayesian-regression/blob/main/report.pdf

Code: https://github.com/NA-Dev/forestfire-bayesian-regression/blob/main/code.pdf

Data Source: http://archive.ics.uci.edu/ml/datasets/Forest+Fires

