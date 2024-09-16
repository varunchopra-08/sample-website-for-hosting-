# sample-website-for-hosting-
A sample static website used for learning hosting on Amazon S3
Certainly! Below is a structured README file you can use for your GitHub documentation on hosting a website using Amazon S3. 

---

# Hosting a Static Website on Amazon S3

## Introduction

This project demonstrates how to host a static website using Amazon S3 (Simple Storage Service), a scalable and durable cloud storage solution provided by Amazon Web Services (AWS). This guide walks through the process of setting up an S3 bucket, uploading website files, and configuring the bucket for static website hosting.

## What is Amazon S3?

Amazon S3 is a cloud-based object storage service with high scalability, durability, and flexibility, making it an ideal choice for hosting static websites. Its global infrastructure ensures that your website can be accessed by users from anywhere in the world.

## Project Overview

In this project, I used Amazon S3 to host my static website, making it publicly accessible online. The steps below outline how I set up the S3 bucket and hosted my website.

## How I Set Up an S3 Bucket

1. **Creating the S3 Bucket**: 
   - Creating the S3 bucket was quick and straightforward; it took me less than two minutes.
   - **Region Selected**: I chose the Asia Pacific (Mumbai) - `ap-south-1` region for efficiency and cost-effectiveness for users based in India. This region ensures low latency and compliance benefits.

2. **Bucket Naming**:
   - It's important to note that S3 bucket names are globally unique. Each bucket name must be unique across all AWS accounts and regions, meaning no two users can have the same bucket name.

## Uploading Website Files to S3

I uploaded the following essential files to my S3 bucket:
- **index.html**: The main HTML page for the website.
- **image assets**: A folder containing images and CSS files for styling the page, as well as JavaScript files for functionality.

## Enabling Static Website Hosting on S3

To make my website public, I followed these steps:
1. After uploading the files, I navigated to the bucket properties.
2. I selected "Edit" and then enabled static website hosting.
3. I specified `index.html` as the index document.

## Access Control Lists (ACL)

An Access Control List (ACL) determines who can access the resources in the S3 bucket. If any object in the bucket needs to remain private, ACLs should be properly configured. ACLs enable different AWS accounts to manage different files within the same bucket.

## Bucket Endpoints

Once static website hosting was enabled, S3 generated a unique bucket endpoint URL. This URL can access the content stored in the S3 bucket through a web browser.

## Troubleshooting

### Error Message: 403 Forbidden

When I first visited the bucket endpoint URL, I encountered the following error:
```
403 Forbidden
Code: AccessDenied
Message: Access Denied
```
This occurred because the HTML and image files I uploaded were still set to private.

### Solution

To resolve this access denial issue and successfully render the website, I updated the ACL settings for the uploaded files to make them public. Once this adjustment was made, the website was accessible.

## Conclusion

Hosting a static website using Amazon S3 is straightforward, especially with the right documentation and tutorials. I took approximately one hour to complete this project while learning about relevant keyword usage in the AWS documentation.

Feel free to reach out if you have any questions or need assistance:

- **Name**: Varun Chopra
- **Email**: varun22chopra08@gmail.com

## Resources
- [Varun's(My) Documentation](https://www.linkedin.com/posts/varun-chopra08_documentation-of-hosting-a-static-website-activity-7241131655069851651-oPRA?utm_source=share&utm_medium=member_desktop)
- [Amazon S3 Documentation](https://docs.aws.amazon.com/s3/index.html)
- [AWS Static Website Hosting](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html)

---



