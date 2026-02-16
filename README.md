Lab 3: Exploratory Data Analysis (EDA)

**Dataset Description**

I am using the **Housing Prices Dataset** for this lab. This dataset provides details on various properties, including their price, area, number of bedrooms, bathrooms, stories, parking, and other amenities like air conditioning and furnishing status.

**Exploratory Data Analysis Findings:**

* **Data Quality:** The dataset is clean with no missing values or duplicate rows.
* **Target Variable:** The target variable is `price`. The distribution of `price` is right-skewed, indicating that while most houses are in a lower price range, there are a few very expensive properties.
* **Feature Relationships:**
* There is a strong positive correlation between `area` and `price`, meaning larger houses tend to be more expensive.
* Houses with more `bathrooms` and `stories` also tend to have higher prices.
* `Furnishing status` affects the price, with furnished houses having the highest average price compared to semi-furnished and unfurnished ones.


* **Goal:** These insights confirm that features like `area`, `bathrooms`, and `furnishingstatus` are significant predictors for building a regression model to predict house prices.
