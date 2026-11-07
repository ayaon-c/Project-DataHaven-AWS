# Project DataHaven: AWS EC2 & S3 Integration

An AWS Cloud Computing project establishing a secure data transfer bridge between an Ubuntu EC2 instance (i-05ccebcbc17dc1a10) and an Amazon S3 bucket (data-haven-project-2026) using IAM roles and AWS CLI.

### Objectives Achieved:
1. Launched an AWS EC2 instance and connected securely via EC2 Instance Connect.
2. Formatted a localized payload file (test.txt).
3. Utilized AWS CLI to securely transfer data to S3 without exposing credentials.
4. Practiced FinOps cost management by safely halting the server (sudo poweroff).

### Commands Executed:
- Create payload: echo "hello data haven" > test.txt
- Secure Transfer: aws s3 cp test.txt s3://data-haven-project-2026/
- Verify Integrity: aws s3 ls s3://data-haven-project-2026/
- Cost protection shutdown: sudo poweroff
