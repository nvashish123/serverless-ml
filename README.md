# serverless-ml
repo to keep artifacts of running ML inferences in Lambda functions in  the serverless manner

comments for serverless-ml.yml -->

1. Replace the CodeBucket and CodeKeyPrefix parameters to your own S3 bucket, where the actual code for the static site will live.
By default, the CFN template reads everything from the website folder from your source S3 bucket and copies into the root level of the target S3 bucket.
This target S3 bucket is the bucket the customer will see in their account, hosting the static web pages.

2. A new lambda function will appear in customers account, which is being used to copy the actual website contents. 


Everything else should just work as-is.

