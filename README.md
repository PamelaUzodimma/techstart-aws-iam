# techstart-aws-iam
# TechStart IAM Project on AWS

This project simulates how a startup company, TechStart Ltd, manages access control for its team using AWS Identity and Access Management (IAM). It demonstrates how to create users, groups, and policies to apply secure, role-based access in the cloud.

## Project Scenario

TechStart Ltd has the following team roles:
- 1 Administrator
- 2 Developers
- 1 Tester
- 1 Read-only Auditor

Each role needs specific access to AWS services. The goal is to give each user the right level of access without exposing unnecessary permissions.

## Objectives

- Create IAM users and organize them into groups
- Write and attach custom IAM policies based on job roles
- Enforce password security and multi-factor authentication (MFA)
- Test and confirm user permissions
- Set up cost alerts using AWS Budgets
- Monitor account activity using AWS CloudTrail

## AWS Services Used

- IAM – Create users, groups, roles, and policies
- S3 – For testing access control (optional)
- EC2 – To simulate developer-level permissions
- CloudTrail – Log and monitor user activity
- Budgets – Create alerts for cost monitoring

## Folder Structure
techstart-aws-iam/
├── policies/              # Custom IAM policy files (JSON)
├── screenshots/           # Setup screenshots (IAM, CloudTrail, Budgets)
├── test-report.md         # Access test results
├── security-config.md     # Password and MFA settings
├── architecture.png       # Project architecture diagram
└── README.md              # This file

## How the Roles Were Set Up
- Admin Group: Full access to all services  
- Dev Group: Access to EC2, S3, and Lambda  
- Test Group: Access to test environments only  
- Audit Group: Read-only access across services

Each user was assigned to a group with a matching policy.
## Testing Access

The `test-report.md` file contains:
- What each user tried to do
- What was allowed or denied
- What policy was responsible for that access level

## Security Measures

- Enabled Multi-Factor Authentication (MFA)
- Created a strong password policy with rotation rules
- Set up CloudTrail to monitor activity logs
- Created a billing alert using AWS Budgets

## What I Learned

- How to design IAM access based on team roles
- How to write and apply JSON IAM policies
- How to test and document cloud permissions
- How to manage cost and monitor user activity on AWS
- How to structure a cloud project for GitHub

## Next Steps

- Convert the setup to Infrastructure as Code (Terraform)
- Add automation using GitHub Actions
- Expand to include more services like CloudWatch and S3 access logging

## Author
Pamela Uzodimma  
AWS Community Builder  
[LinkedIn](https://www.linkedin.com/in/pamela-uzodimma)  
pamelauzodimma@gmail.com
