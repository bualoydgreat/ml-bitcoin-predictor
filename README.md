# Bitcoin Predictor for Machine Learning Regression Samples
Bitcoin is a decentralized digital currency created in January 2009. It follows the ideas set out in a white paper by the mysterious and pseudonymous Satoshi Nakamoto. The identity of the person or persons who created the technology is still a mystery. Bitcoin offers the promise of lower transaction fees than traditional online payment mechanisms do, and unlike government-issued currencies, it is operated by a decentralized authority. (ref. Investopedia)

This Bitcoin Predictor uses a [data](/Data/BitcoinHistoricalData.csv) with 3245 days of Trading properties such as:  
- Date (str, date time): Time of measurement
- Price (float): Price of Bitcoin at the end of the day (midnight)
- Open (float): Price of Bitcoin at the start of the day (midnight)
- High (float): Highest price of Bitcoin during the day
- Low (float): Lowest price of Bitcoin during the day
- Vol. (float): Approximated count of transactions (Buy/Sell) of Bitcoin
- Change % (float, percentage): Percentage between the Price and Open


## Conclusion
The Linear Regression and Bayesian Ridge both produced promising models which in turn may be overfitting. The decision tree produced the best result at a relatively low depth of 50. It produced a low correlation at r2 score at 0.37 because the model was not trained to predict higher price labels and maxes out at the price spike during early 2018. 

The Bitcoin and most of the cryptocurrency are volatile enough to cause false assumptions and predict wrong results. The statistical models could only be used as an indicator guide to increase chances of the goals already set earlier.
<center>
    <h2>SUMMARY OF RESULTS</h2>
  
</center>

|Machine Learning Method| RMSE | R2 Score | Targeted Parameter
| :---: | :---: | :----: | :----: |
| kNN | 19590.21 | 9% | n_neighbor = 21
| Linear Regression | 462.98 | 100% | Auto
| Bayesian Ridge | 463.54 | 100% | tol = 1e-6 
| SVR | 26277.09 | -64% | C = 100
| Gradient Boosting | 16495.23 | 35% | learning_rate = 0.1
| Decision Tree | 16325.28 | 37% | max_depth = 50
| Random Forest | 16391.62 | 36% | n_estimators = 30
  
## Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

## License
Distributed under the [MIT](https://choosealicense.com/licenses/mit/) License.
