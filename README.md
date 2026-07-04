## commands for dvc:

### 1. To initialize dvc:
 dvc init


### 2. to add data into dvc:
 dvc add path-to-your-data-file     eg: data/wine_samples.csv


### 3. adding remote origin: eg: s3 bucket:
 dvc remote add -d wineremote s3://mlops-demo-abhishek-dvc-bucket       wineremote is just a name; 

### 4. pushing to remote origin:
 dvc push

## Note: 
you need to have aws account and configured in your CLI; aws configure in your cli and enter access key and secret access key

if you make any change in your data/csv file, you need to 2 and 4, you should also git commit your dvc configs


