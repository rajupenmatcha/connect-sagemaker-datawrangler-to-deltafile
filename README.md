# connect-sagemaker-datawrangler-to-deltafile

You might have your data file stored on Delta lake and would like to connect to it from Amazon SageMaker.

The notebook in this repository shows how you can do just that.

The steps are as follows:
1. Load your CSV file to spark context and write a S3 manifest file

2. Upload the manifest file and other related files to your S3 bucket

3. Create a Athena table that can read from this S3 bucket

4. Connect to this delta file using the Athena connection in SageMaker Data Wrangler