# This contains the M10 Assignment 

Files loaded in S3 bucket:
==========================
S3 URI: s3://ia-module10/charities_bureau_scrape_allpage_group3_20240414144109.csv

URL: https://ia-module10.s3.amazonaws.com/charities_bureau_scrape_allpage_group3_20240414144109.csv

S3 URI: s3://ia-module10/charities_bureau_scrape_group3_20240414143925.csv

URL: https://ia-module10.s3.amazonaws.com/charities_bureau_scrape_group3_20240414143925.csv


Update S3 bucket policy:
========================

{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "AllAccess",
            "Effect": "Allow",
            "Principal": "*",
            "Action": [
                "s3:ListBucket",
                "s3:PutObject",
                "s3:GetObject"
            ],
            "Resource": [
                "arn:aws:s3:::ia-module10",
                "arn:aws:s3:::ia-module10/*"
            ]
        }
    ]
}