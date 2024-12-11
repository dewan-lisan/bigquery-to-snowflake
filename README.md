# bigquery-to-snowflake

## Create snowflake storage integration
```
CREATE STORAGE INTEGRATION gcs_int
  TYPE = EXTERNAL_STAGE
  STORAGE_PROVIDER = 'GCS'
  ENABLED = TRUE
  STORAGE_ALLOWED_LOCATIONS = ('gcs://ls_gcs_int_stage/securities_balance/')

-- the bucket is created by this command

DESC STORAGE INTEGRATION gcs_int;
```
