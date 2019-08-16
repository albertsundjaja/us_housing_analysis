# US House Price Analysis

## Dataset

This project uses the Ames Housing dataset http://jse.amstat.org/v19n3/decock.pdf

The dataset is available on Kaggle https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data

The train data contains 1460 rows with 81 columns, and the test data contain 1459 and 80 columns (minus the target column)

### Quality

There are a number of columns with missing values such as `LotFrontage, Alley and Fence`, however, these missing values might not be an indication of error, it might be that the property simply does not have a fence for example. As such, we need to take great care in imputing these missing values.

## Visualization

### Price Distribution for 1 - 3 Bedrooms

We will start with looking at how the number of bedrooms affect the properties price. Below is a chart for each of 1 - 3 Bedrooms properties price distribution.

![price_distribution_br_1](img/price_distribution_br_1.png)

It is unexpected to see that they all have similar prices despite the different in number of bedrooms. We will investigate this further by combining the distribution into a single chart.

![price_distribution_br_2](img/price_distribution_br_2.png)

From the chart above, we could see that the 2 bedrooms properties (green) actually have lower mean in the price distribution compared to properties with 1 bedrooms (orange). This indicate that number of bedrooms is not the only factor in determining the property price.

Intuition tells that perhaps properties with 2 bedrooms are located farther away from the CBD where land price is cheaper, hence larger properties size.

