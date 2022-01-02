## Dataset Info

This dataset is a sample taken from the `san_francisco_311.311_service_requests` dataset found on Google Cloud BigQuery: `bigquery-public-data.san_francisco_311.311_service_requests`.

It uses 311 calls data from the 11th of June 2021. 

You can recreate the dataset from the source using the following query:

```sql
SELECT
  *
FROM
  bigquery-public-data.san_francisco_311.311_service_requests
WHERE DATE(created_date) = '2021-06-11'
```

Note that the source dataset might have changed in the meantime as it is not a static dataset, it is continuously being updated by the maintainers. 

Please refer to my [blog post](https://lucytalksdata.com/introduction-to-geopandas-analysing-311-call-data/) for an in-depth guide on how to visualise this data using GeoPandas. 
