import pandas as pd
grocery = pd.read_csv("groceries.csv")
grocery.head()
grocery.groupby('product_description')['price'].mean()
grocery["price_new"] = grocery['price'].fillna(
   grocery.groupby('product_description')['price'].transform("mean")
)
grocery[grocery["price"].isna()].head()