# Kings County House Sales Analysis



#### Authors: Maureen Kitang'a, Samuel Kyalo, Priscila Kamiri, Leo Kariuki, Jimcollins Wamae & Steve Githinji

This project is a part of the [Data Science (DSF-FT) Course](https://moringaschool.com/courses/data-science-course/) at [Moringa School](https://moringaschool.com/). The full project description can be found [here](https://github.com/learn-co-curriculum/dsc-phase-2-project-v2-3).

## Overview
Real estate developers are interested in identifying factors that influence the sale price of homes in King County, as well as developing models to predict the sale price of homes based on these factors. This information can be used to optimize the design and marketing of new properties, identify investment opportunities, and make data-driven decisions about the development and sale of properties. 




## Business Problem
The stakeholder is a Real Estate Developer in a northwestern county who identifies and acquires land for new development projects, as well as oversees the construction process from start to finish. The Real Estate developer want to gain market insights that will lead to an increase in house sales.



## Data
This project uses the [King County House Sales dataset](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction). The dataset contains information on over 21,000 home sales in King County, Washington, USA between May 2014 and May 2015. The dataset includes a variety of features such as the number of bedrooms and bathrooms, the size of the property, the location of the property, and various other attributes that may influence the sale price of a home.



## Method

Regression was the algorithm used in building the models. First, we built the baseline model with price as the target variable and sqm_living as the predictor.
Then we proceeded to add more features and fitted another model which was better than the first one. Since, we had a target for our variance in price, we fitted the final model.

## Results

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


## Repository Structure

![repository structure](images/Capture.PNG)




