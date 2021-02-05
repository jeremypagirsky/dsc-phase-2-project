# Predicting Seattle Housing Prices

**Author**: [Jeremy Pagirsky](https://github.com/jeremypagirsky)

## Overview

Like many American cities, housing in Seattle is becoming increasingly more expensive. According to [Norada](https://www.noradarealestate.com/blog/seattle-real-estate-market/), median housing prices in the city have appreciated about 118% since 2012, from 355,000 to 773,508 dollars. This can put great pressure onto many of its working residents to afford the steeply increased cost of living.

This project attempts to illumine the factors associated with housing price increases in Seattle for those looking to purchase a new home. In particular, this project will attempt to ascertain which zip codes may play a role in housing prices.

## Data

Data on about 21000 homes in King County up to the year 2015 was supplied by the Flatiron School.

## Methods

Homes in Seattle were selected out of the original dataset. The primary statistical method was Linear Regression using Statsmodels OLS and Scikit Learn train-test splits and cross-validation. Main statistics of examination were $R^{2}$, mean absolute error, and root mean square error.

## Results

The largest predictor for housing prices is a home's square footage.
![square_feet](./images/sqft_price.png/)

The majority of zip codes in Seattle also predicted housing prices.
![zip_codes](./images/zips.png/)

## Conclusions

- **Larger homes are expected to be more expensive.** This model demonstrates a strong relationship between square footage and housing price. One may expect larger homes to be more expensive and smaller homes to be less expensive in Seattle.

- **Search for homes in zip codes expected to have lower prices**. For individuals seeking more affordable housing options, this model predicts the following zip codes to decrease a home's price relative to other zip codes: 98106, 98118, 98168, 98178, 98198.

## Future Work

Further analyses may consider the following for deeper insights into this model:

- **Examine prices by council district.** This model may warrant the need to expand from zip code to council district. This could be illuminate political implications for metropolitan area housing.
- **Generalizability to King County.** While this model may be useful in predicting prices for Seattle, it is uncertain whether or not this model may be useful for the entirety of King County.
- **Incorporate additional features.** To gain more clarity on prices, it may be useful to gain an understanding of other factors relevant to a home, such as relative size compared to neighbors and recency of renovations.


## For More Information

Please review the full analysis in [the Jupyter Notebook](./Seattle_Housing_LR_Model.ipynb) or the [presentation](./Seattle_Housing_Price_Prediction.pdf).

For any additional questions, please contact ***Jeremy Pagirsky (jeremy.pagirsky@gmail.com)**

## Repository Structure

```
├── Seattle_Housing_README.md               <- The top-level README for reviewers of this project
├── Seattle_Housing_LR_Model.ipynb          <- Narrative documentation of analysis in Jupyter notebook
├── Seattle_Housing_Price_Prediction.pdf    <- PDF version of project presentation
├── data                                    <- Both sourced externally and generated from code
└── images                                  <- Both sourced externally and generated from code
```