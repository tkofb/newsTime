# newsTime

## overview

this project studies to what extent someone could use the employment rate to price a currency and use that to evaluate whether or not it was overvalued

## abstract

using the unemployment rate solely is not enough to value a pair and there should be additional data points to drive your pricing model

## key findings

- given the high degree of precision in regards to currencies, (e.g. USD/EUR today is .96611) the unemployment rate is not able to accurately price a pair given its less precise measurement.
- when we split our data into train and test datasets and evaluated it with a regression line we were able to rank our pairs in regards to their correlation score and MSE as such, and we saw low correlation between the two given the precision needed in most cases.
	- GBP/USD
		- R2: 0.702541002750887
		- MSE: 0.0035444671234330857
	- AUD/USD
		- R2: 0.6953667652484221
		- MSE: 0.0008801397455916797
	- EUR/USD
		- R2: 0.00205594147734057
		- MSE: 0.44147806372461085
	- USD/JPY
		- R2: 0.2883402303162542
		- MSE: 117.19229316794274
			- keep in mind that USD/JPY is priced differently than on average (in the hundreds)
	- USD/CHF
		- R2: -0.2394778469677885
		- MSE: 0.0029581351445620886
- some of the pairs are correlated as you may expect. For example GBP/USD and EUR/USD were very correlated.
- overall we are not able to use unemployment rate solely, given that the correlation would have to be really high as this is in regards to forex. Movement from 1.4000 to 1.4001 actually has a potentially big impact given the case that this is often a leveraged investment. Therefore we would have to add other variables in most cases to potentially create a better model.

## study

[forex study](https://tkofb.github.io/)

## license

[MIT](https://choosealicense.com/licenses/mit/)
