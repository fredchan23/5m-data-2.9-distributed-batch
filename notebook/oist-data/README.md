# Olist Dataset Setup

The CSV files used by `notebook/oist_spark_analysis.ipynb` are not intended to be committed to the GitHub repository.

Before running the notebook, download the Olist Brazilian E-Commerce dataset from Kaggle:

https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## Required files

After downloading and extracting the archive, place these CSV files in this folder:

- `olist_customers_dataset.csv`
- `olist_geolocation_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_order_payments_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_orders_dataset.csv`
- `olist_products_dataset.csv`
- `olist_sellers_dataset.csv`
- `product_category_name_translation.csv`

## Expected location

Keep the files in:

`notebook/oist-data/`

The notebook loads them with relative paths such as:

```python
data_dir = 'oist-data'
customers = spark.read.csv(f'{data_dir}/olist_customers_dataset.csv', header=True)
```

If any file is missing or stored in a different location, the notebook will fail when reading the datasets.
