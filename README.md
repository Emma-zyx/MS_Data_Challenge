## MS_Data_Challenge

The 2nd Summer Data Challenge is held by Morgan Stanley in 2021, for Columbia IEOR students to participate. It is an equity research project with both quantitative and qualitative facets, and students need to apply AI/ML techniques on public data to analyze American Airlines, Disney, and PepsiCo stock price changes compared with S&P 500 from 2010 to 2021. Each team needs to collect relevant data, specify main drivers behind stock prices changes, and explain results to business executives at Morgan Stanley. <br>

Our team collect both news and social medai data using APIs to obtain more comprehensive perspectives.<br> 
Below is our steps to conduct this project.
- We first split periods for three companies respectively based on 50-day moving averages of stock returns. The table is a summary table for three companies’ stock performances.
  - American Airlines has 4 time periods: 
    - 2013.12 - 2014.12; 2015.01 - 2018.12; 2019.01 - 2019.12; 2020.01 - 2021.07
  - Disney has 4 time periods: 
    - 2010.01 - 2015.06; 2015.06 - 2017.06; 2017.06 - 2019.06; 2019.06 - 2021.07
  - PepsiCo has 6 time periods: 
    - 2010.01 - 2011.06; 2011.06 - 2013.06; 2013.06 - 2015.06; 2015.06 - 2018.01; 2018.01 - 2019.01; 2019.01 - 2021.07
![Image](https://github.com/Emma-zyx/MS_Data_Challenge/blob/main/Picture2.png)
- Then, we conduct XGBoost tree models to check feature importance for each period.
  - Our process flow for each model in a period is below. 
  ![Image](https://github.com/Emma-zyx/MS_Data_Challenge/blob/main/Picture1.png)
- After getting all the feature importances of each period, we made a live picture to show how influential features changes over time in the slides. 

Notes:
- The complete model code for Disney is in DIS_FINAL.ipynb.
- Please refer to details in the slides.
