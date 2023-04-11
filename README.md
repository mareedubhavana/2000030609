#  building a analytical ecommerce webpage through any aws service
For most applications, websites can run with only client side code and be comprised of only HTML, CSS and JavaScript. Such websites are usually defined as static websites. With no server side code to run or maintain there is no point in using conventional web servers.Amazon Web Services (AWS) offers multiple options for hosting static or dynamic websites. For static content, the simplest and most affordable option is the Amazon Simple Storage Service (S3).You can store any number of objects in a bucket and can have up to 100 buckets in your account. S3 supports only static websites. However, if you're looking to host a dynamic website, then you can use services like EC2 or RDS for server-side processing and databases.

#code
{
    "Version": "2023-04-11",
    "Statement": [
        {
            "Sid": "AllowPublicRead",
            "Effect": "Allow",
            "Principal": {
                "AWS": "*"
            },
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::csc-30609/*"
        }
    ]
}

1. open aws management console
2. search s3 storage in console search
3. open s3 and create bucket
4.name of the bucket:
5. click on acl's enabled
6.create bucket
7. open the created bucket in the console and add folder into the bucket
8.now wait for uploading
9. enable static web hosting and run the bucket in a browser
