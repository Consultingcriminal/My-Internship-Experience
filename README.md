<br />
  <h2 align="center">My Summer Intership Experience</h2>

  <p align="center">
    As a Data Science Intern At Hero Steels Ltd.
    <br />
  </p>
</p>

<h2>Overview</h2>

In the Summer of 2020,I got an oppurtunity to work as a Data Science Intern for a major steel producer of the country.
\
During my tenure as an intern,I re-implemented the paper-
[AI in Healthcare: Time-Series Forecasting Using Statistical, Neural, and Ensemble Architectures]( https://www.frontiersin.org/articles/10.3389/fdata.2020.00004/full ) for predicting the steel production over the next 3 months.



<!-- ABOUT THE PROJECT -->
<h2>Problem Statement for the Prediction Task</h2>

The task at hand was to predict the steel production of the organization over the next 3 months .An uni-variate time-series of the organisational steel output over the past 48 months was provided for the purpose of model training.

### Model Architecture:

* The final model consisted of an **ensemble** of 3 Models namely **ARIMA,ANN and a multi-variate LSTM.**
* **Hyperopt And Keras Tuner**  were used for minimizing the cost func = **(RMSE/10 + (1-R_squared))** in the respective models.



<h3>Feature Selection For LSTM model</h3>

An assumption to consider the problem as a **regressive problem** was made. An **XgBoost Regressor** was used to model the feature importance.The top selected features are as follows-

* DollarVsRupees
* A Public Sector Steel Company Shares Price
* A Top Private Sector Steel Company Shares Price
* Price of Crude Oil
* Price of Iron Ore
* Price of Natural Gas
* Price of Coal

The above features were used for training the LSTM model including the original production time-series,making this a many-to-one sequence prediction problem.

<h3>Results</h3>

* Initial monthly variance = 1962 units

* Blending Weights
    * ARIMA = 0.29
    * ANN = (-)0.07
    * Multi-variate LSTM = 0.12

*  Predicted monthly variance by the model = 736 units (Almost 60% reduction in variance)  

### Built With

This section should list any major frameworks that you built your project using. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.
* [Tensorflow](https://www.tensorflow.org/)
* [XgBoost](https://xgboost.readthedocs.io/en/latest/)
* [HyperOpt](https://hyperopt.github.io/hyperopt/)
* [Stats_Models](https://www.statsmodels.org/stable/index.html)





<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [Research Paper]( https://www.frontiersin.org/articles/10.3389/fdata.2020.00004/full)
* [Kaggle](https://www.kaggle.com/)
* [Machine Learning Mastery](https://machinelearningmastery.com/)
* [KDnuggets](https://www.kdnuggets.com/)





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
