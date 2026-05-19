# AWS Static Website Hosting with S3 and CloudFront

Static resume website deployed manually on AWS using S3, CloudFront, Route 53, ACM, and IAM/security best practices.

This project is part of my transition from Automotive ECU Validation & Verification into Cloud/DevOps.

## Project Goal

The main focus of this project is to understand AWS deployment architecture, including S3 static hosting, CloudFront, Route 53, ACM, and basic IAM/security best practices.

## Phase 1: S3 and CloudFront Hosting

- Created a private Amazon S3 bucket to store the static resume website files.
- Uploaded the initial `index.html` file while keeping direct public access blocked.
- Created an Amazon CloudFront distribution in front of the private S3 bucket to serve the website securely.
- Configured CloudFront access to the S3 origin so the website is publicly available through CloudFront while direct S3 access remains blocked.
- Set `index.html` as the default root object so the CloudFront root URL loads the homepage correctly.
