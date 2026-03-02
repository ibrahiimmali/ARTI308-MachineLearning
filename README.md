Lab 4: Data Quality Assessment & Preprocessing
Dataset Description
I am using the Housing.csv Dataset, which contains 545 entries and 13 features. It includes house details like price, area, and various amenities.

Preprocessing Findings:

Data Quality: Identified scale inconsistencies (millions vs. units), extreme outliers in price, and categorical text features requiring encoding.

Missing Values: Introduced and then handled missing data in the area column using Median Imputation to ensure a robust center point unaffected by outliers.

Outlier Management: Used the Interquartile Range (IQR) method to remove 15 extreme price points, stabilizing the dataset from 545 to 530 rows.

Normalization: Applied Min-Max and Z-score scaling to price and area to bring features into a comparable range for modeling.

PCA: Reduced six numerical features into two principal components, capturing 62.9% of the total variance.

Goal:
These steps clean and standardize the data, making it ready for high-performance regression or clustering models.
