## View all running services on AWS

**AWS Resource Explorer** the best place to see all the **services running and resources allocated**. It allows to **filter** by **type** and by **region**. The only issue is it may take some time to finish indexing all the resources.

Link: [https://resource-explorer.console.aws.amazon.com/](https://resource-explorer.console.aws.amazon.com/)

[![enter image description here](https://i.stack.imgur.com/wp49X.png)](https://i.stack.imgur.com/wp49X.png)


## Deleted S3 buckets - AWS Region Not Found
You may be experiencing some lag.

Amazon S3 is built on eventual consistency model, it can take some time for changes to propagate across all AWS Regions. This is why you might temporarily see your bucket in the console, or in a response to a ListBuckets API request, even after you delete the bucket. Until the bucket is completely removed by Amazon S3, you might still see the bucket, but you can't perform any other actions on the bucket.

As it states in this answer here
