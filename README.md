# Cloud Computing Project - 2

## Group Members

1. Avinash Kodali
2. Manogna Pagadala
3. Manaswi Kommini

## AWS Credentials

1. Access key ID - AKIAX643R3BDZ34JHUR2
2. Secret access key - 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

## S3 Bucket Names

1. cc-project-input-bucket
2. cc-project-output-bucket

Our cloud app will implement a smart classroom assistant for educators. This assistant takes videos from the user’s classroom, performs face recognition on the collected videos, looks up the recognized students in the database, and returns the relevant academic information of each student back to the user.

Steps to setup:
Created input and output S3 buckets.
Created the dynamo_db table and loaded the data from the “student.json” to the table.
Install the Docker Desktop and create a docker image by using the command “docker build.”
After the image is created, get the latest image and tag the image using the “docker tag“ command. By using the command “docker push ” push the image to the ECR repository.
Lambda function is created from the deployed image from the ECR Repository and an S3 input bucket event trigger is created.
In the workload generator set the input and output bucket names accordingly and run the
workload generator for both the test cases
