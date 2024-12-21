# future-demand-prediction
Predicting future demand for product optimization - A retail supermarket
This is a dataset containing information about the business activities of a retail supermarket in the United states. The dataset was gotten from kaggle

The data consists of 13 features and 9994 observations with the information of a retail supermarket in different parts of the united states The features are

Ship mode: The type of shipping a customer prefers when he/she makes a purchase
segment: the category of customer who made the purchase
city and state: The city and state where the customer made the purchase
Region: the region in the US where the customer made the purchase from
category and sub-category: the category and sub-category of product a customer purchased
sales: the amount realised from the sale of products after the discount has been deducted
quantity: the unit of product purchased
discount given to customers for each sale
profit realized from each sale

The following new features were created to get a better understanding of the data, capture relationships and get an accurate prediction:

Actual total sales - The total sales for every purchase before the discount was applied
unit sale - the unit price for each product
Discount price - The discount amount on the total sales for every purchase


Other steps taken include:

The dataset was segmented by category, segment, sub category and ship mode and each segment was analyzed
There were a few products with very high total sales
The distibution of numerical features were imbalanced and these features were deskwed and normalized
Categorical features were encoded using the OneHotEncodre algorithm
The Recurrent feature elimination algorithm was used to select features that were relevant for the prediction

Decision tree - The decision tree model is capable of handling complex, non - linear relationships, such as the relationship between various products, their prices and the quantity purchased. The decision tree consists of several node. Each node consists of a number of features that are randomly selected. The model checks the relationship between each node and the target variable and trains the model using the best best features selected from different nodes with a tree depth of 10, min sample node of 10, min sample, and max features of 5 for the leaf node.
Random forest - The random forest model is also capable of handling complex, non - linear relationships, such as the relationship between various products, their prices and the quantity purchased. It is an ensemble technique where the model consists of many decision trees as against a single one. It averages the results from all trees to obtain the final prediction. A number 0f 500 trees were used in the forest, with a tree depth of 10, min sample node of 10, min sample, and max features of 5 for the leaf node.
