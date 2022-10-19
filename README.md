# About the Dataset
Zomato is the leading food delivery and restaurant rating app in India. Although the food
delivery feature is restricted to India, the dine-out feature is spread over 19 countries. Zomato’s
dining-out feature includes providing restaurant information (cuisines, menu, approximate cost,
etc.), table reservation, user ratings and reviews on the app.
We use this Zomato Restaurants Dataset, available on Kaggle, in order to determine which
features of the restaurants affect the restaurant’s rating, and by how much using statistical
methods.

Source : https://www.kaggle.com/datasets/shrutimehta/zomato-restaurants-data?select=zomato.csv

# File Structure
```bash
├── LICENSE
├── README.md
├── data
│   ├── zomato.csv
│   └── zomatoClean.csv
└── source
    ├── ZomatoAnalysis.ipynb
    └── ZomatoEDA.ipynb

2 directories, 6 files
```

# File Descriptions

**data**:
- zomato.csv : this is the orignal data file downloaded from Kaggle and is provided as input to ZomatoEDA.ipynb
- zomatoClean.csv : this is the cleaned dataset, which is the input for ZomatoAnalysis.ipynb

**source**:
- ZomatoEDA.ipynb : Jupyter Notebook file with initial analysis of the dataset. The process followed for cleaning the data is also described here.
- ZomatoAnalysis.ipynb : Jupyter Notebook file with the main Analysis with all the statistical tests and regression analysis performed

# Project Process

## Questions explored
1. Do the ratings of expensive restaurants significantly differ from the ratings of
inexpensive restaurants?
2. Does providing an online delivery service significantly affect the ratings?
3. Does providing online table reservations affect the ratings?
4. How does cuisine affect the restaurants’ ratings?
a. Are multi-cuisines restaurants rated higher than single-cuisine restaurants?
b. How do the ratings compare for the Top 5 individual cuisines?
5. How do food chains compare to stand alone restaurants in ratings?
6. Can we build a linear model for the average ratings of a particular restaurant given the
above characteristics?

## Statistical methods used
1. Hypothesis Testing
a. Two sample two-tailed z-test
b. Two sample one-tailed z-test
2. ANOVA
3. Confidence Interval Testing
4. Multiple regression analysis

# Findings

1. Expensive restaurants have significantly higher ratings as compared to inexpensive
restaurants.
2. Restaurants having an online delivery option have significantly higher ratings.
3. Restaurants providing table reservations have significantly higher ratings.
4. Stand alone restaurants have significantly higher ratings than food chains.
5. Multicuisine restaurants have significantly higher ratings.
6. Among single cuisine restaurants, there is a significant difference between their mean
ratings.


# Future Work

I am currently working on understanding the affect of number of reviews on each of the variables.
