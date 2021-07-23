## Create a CI/CD Pipeline using AWS Code* tools for Amazon Managed Workflow for Apache Airflow (MWAA)

This repository contains a AWS CloudFormation template that automates the creation of a AWS CodeCommit Repository and AWS CodePipeline pipeline that would be used to do CI/CD to an S3 Bucket that would be used as the source for an Amazon Managed Workflow for Apache Airflow environment(MWAA). Follow the blogpost to get step by step guideline on creating a resources.

### Prerequisites
You must already have the following:
A. Source artifacts for your Airflow project. In the following example, I have configured the following subfolders:
    a. dags/ for my Apache Airflow DAGs
    b. plugins/ for all of my Plugin zip files
    c. requirements/ for my requirement.txt files
B. An IAM role that has access to run AWS CloudFormation and to use CodeCommit & CodePipeline

### Detailed Steps
 Step 1: Zip your artifacts and upload them to your S3 bucket configured for MWAA
 Step 2: Run AWS CloudFormation to AWS CodeCommit Repository and CodePipeline
 Step 3: Verify by making a change to a DAG file the newly created CodeCommit Repository

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

