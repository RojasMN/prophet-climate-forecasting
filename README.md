# **Climate Forecasting Model with Prophet: Exploratory Data Analysis and Statistical Comparison**
---
- The dataset consist of 4 parameters (mean temperature, humidity, wind speed, and mean pressure) measured during a period of 5 years approximately. The objective of this project is to develop a forecasting model that can predict the values of a variable of interest, in this case, temperature. To achieve this, we will first conduct an exploratory data analysis to understand the characteristics of the data.  We will then utilize the Prophet package to construct a predictive model, incorporating additional variables such as humidity and average pressure to enhance the model's performance. Finally, we will perform a statistical analysis to compare the model's performance with and without the additional regressor variables.
- The dataset used in this project was obtained from: https://www.kaggle.com/datasets/sumanthvrao/daily-climate-time-series-data

### **Conclusions and Summary of the Results**
---
- Initially, we performed an exploratory data analysis to identify interesting correlations between the various parameters in the database. We modified and created auxiliary variables to facilitate the visualization of seasonal and annual trends. We selected the most important variables for building the predictive model, excluding those that did not provide relevant information for predicting the variable of interest. We determined that there is a slight upward trend in temperature and a slight downward trend in humidity over the years, using tools such as seasonal decomposition and correlation analysis.
- We found a strong negative correlation between humidity and temperature, which is amplified during months typically known to be hot and dry. Temperature also showed a moderate positive correlation with wind speed. Together, these variables proved useful for constructing the predictive model.
- Using Prophet, we initially built a simple model trained solely with temperature data. Subsequently, we added humidity and wind speed as regressor variables, thereby improving the model's performance (measured using parameters such as mean squared error and R squared).
- Finally, considering that the residual values should exhibit a normal distribution, we compared the residual distribution between the two constructed models. Consistent with previous results, the model with regressor variables showed, on average, residuals of smaller magnitude. Using QQ plots, we confirmed that both models presented a normal distribution of residuals.

  
