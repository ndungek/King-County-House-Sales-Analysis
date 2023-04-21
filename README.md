# Kings County House Sales Analysis



#### Authors: Maureen Kitang'a, Samuel Kyalo, Priscila Kamiri, Leo Kariuki, Jimcollins Wamae & Steve Githinji

This project is a part of the [Data Science (DSF-FT) Course](https://moringaschool.com/courses/data-science-course/) at [Moringa School](https://moringaschool.com/). The full project description can be found [here](https://github.com/learn-co-curriculum/dsc-phase-2-project-v2-3).

## Overview
Real estate developers are interested in identifying factors that influence the sale price of homes in King County, as well as developing models to predict the sale price of homes based on these factors. This information can be used to optimize the design and marketing of new properties, identify investment opportunities, and make data-driven decisions about the development and sale of properties. 




## Business Problem
The stakeholder is a Real Estate Developer in a northwestern county who identifies and acquires land for new development projects, as well as oversees the construction process from start to finish. The Real Estate developer want to gain market insights that will lead to an increase in house sales.



## Data Understanding
This project uses the [King County House Sales dataset](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction). The dataset contains information on over 21,000 home sales in King County, Washington, USA between May 2014 and May 2015. The dataset includes a variety of features such as the number of bedrooms and bathrooms, the size of the property, the location of the property, and various other attributes that may influence the sale price of a home.


## Modeling
In this section, we shall be building the models.

We will first start by building a baseline model. The baseline model will be used to compare the performance of the other models that we will be building. After that, we will build our multiple linear regression model.

#### Build Baseline  Model


The target variable is price. Therefore, we look at the correlation coefficients for all of the predictor variables to find the one with the highest correlation with price.

Our most strongly correlated variable with `price` is `sqm_living`

The model is statistically significant as it explains only 49.3% of the variance in the data. However, it is a good starting point for our analysis. Each prediction is off by about $173,829.
  
  - The coefficient of `sqm_living` is about \$3023. This means that for every square meter increase in the house, the price of the house increases by about \$3023.

#### Build Iterated Multiple Linear Regression Model 1
> We will now iterate the baseline model by building a multiple linear regression model that will have more than one independent variable.

All of the coefficients are statistically significant, and explains about 65% of the variance in price. Each prediction is off by about $ 140,692.20

#### Build Iterated Multiple Linear Regression Model 2
> We will now build another iterated model.

##Final Model Regression Results

The results showed that:

1. A one-unit increase in the number of bathrooms is associated with an increase of $16,410.00 in home price.
2. A one-unit increase in square metre of living space is associated with an increase of $ 2813.50 in home price.
3. A one-unit increase in square metre of the lot size is associated with a increase of $ 2.9292 in home price.
4. A one-unit increase in the square metre of the basement is associated with an decrease of $ 663.40 in home price.
5. A one-unit increase in the year the home was built is associated with a decrease of $ 838.71 in home price.
6. Compared to zipcode_98103, zipcode_98004 has the highest increase of $462,900 in home price.
7. Compared to zipcode_98103, zipcode_98092 has the highest decrease of $381,700 in home price.

## Conclusions
Multiple Linear Model 2 was chosen as the final model. This is beacause it explained about 74 % of the variance in price, about 10% more than Multiple Linear Model 1. It also had a lower Mean Absolute Error, by about $ 32,000.

From the final model, bathroom is associated with bringing the highest increase in sale price.

An increase in sqm_living count by 1 unit had the second highest associated increase in price.

Compared to zipcode_98103, zipcode_98004 has the highest increase of $462,900 in home price.

## Recommendations
When building new houses, The Real Estate Developer should therefore prioritize:

increasing the number of bathrooms,
consider the size(square meters) of the living space
consider building houses in the postal area of zipcode_98004



### Next Steps

A further study may be required with a larger dataset for better insights.

More factors like the population in each area may be considered



## For More Information

See the full analysis in the [Jupyter Notebook](https://github.com/ndungek/King-County-House-Sales-Analysis/blob/main/index.ipynb) or review this [presentation](https://1drv.ms/b/s!AiNhn0lGIhsp9E25Dqx67QjOwUSB?e=mVayGL).

Contact me: ndungek66@gmail.com




