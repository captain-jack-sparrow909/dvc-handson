## commands for dvc:

### 1. To initialize dvc:
 dvc init


### 2. to add data into dvc:
 dvc add path-to-your-data-file     eg: data/wine_samples.csv


### 3. adding remote origin: eg: s3 bucket:
 dvc remote add -d wineremote s3://mlops-demo-abhishek-dvc-bucket       wineremote is just a name; 

 for an existing project to know what remote origin is used check this file -> .dvc/config

### 4. pushing to remote origin:
 dvc push

## Note: 
you need to have aws account and configured in your CLI; aws configure in your cli and enter access key and secret access key

if you make any change in your data/csv file, you need to 2 and 4, you should also git commit your dvc configs

## summary:
data is stored in s3 bucket and meta-data of the dataset is stored in git
to the git -> .dvc folder and your data.csv.dvc file should be pushed
in the data.csv.dvc is the checksum which is pointing to the latest data available in the s3 bucket

