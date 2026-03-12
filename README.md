# Lab 5: Feature Engineering for Classification

## Dataset Description
The `talabat_enhanced_orders.csv` dataset contains 100,000 rows and 23 columns representing food delivery orders placed across multiple Egyptian cities. Features include order details (item name, quantity, total price), timestamps, GPS coordinates for the restaurant, customer, and driver, traffic level, driver availability, and the target variable `Order_Status` (Delivered, Cancelled, In Transit).

## Lab Focus
Unlike data cleaning labs, this dataset required no preprocessing — there were no missing values or duplicate rows. The entire focus was on **feature engineering**: transforming raw columns into more informative inputs before training a classifier.

## Feature Engineering
Three categories of features were engineered from existing columns:
- **Time-based:** hour of day, day of week, weekend flag, and peak-hour indicator — all extracted from `Order_Time`
- **Price-based:** `price_per_item` (Total_Price / Quantity) and a bucketed `price_tier` (low, medium, high, very high)
- **Distance-based:** Haversine straight-line distance between the restaurant and the customer, complementing the road-based `Delivery_Distance_km` already in the dataset

## Leakage Awareness
Columns unavailable at order placement time — `Delivery_Time` and `Delivery_Duration_Minutes` — were excluded to prevent data leakage. ID columns were also dropped as they carry no generalizable signal.

## Baseline Model
A **Random Forest** classifier was trained using a pipeline that one-hot encodes categorical features and passes numeric features through unchanged. The model used `class_weight="balanced_subsample"` to partially address class imbalance. Baseline accuracy reached **~85.2%**, which reflects the majority class proportion rather than genuine performance across all classes.

## Feature Importance
The top features by importance were spatial and price-based: driver-to-restaurant distance, price per item, total price, and GPS coordinates. Engineered features ranked among the highest, confirming that the feature engineering step added real predictive value. Time flags and item category features ranked much lower.

## Goal
The goal of this lab was to practice transforming a clean, real-world-style dataset into a well-structured feature matrix suitable for classification. After engineering and encoding, the dataset was evaluated using both accuracy and per-class metrics, with feature importance used to assess which transformations were most effective.
