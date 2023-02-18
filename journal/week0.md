# Week 0 — Billing and Architecture
Tasks completed:
- watched all videos
- set up MFA on AWS root account
- added credits to account
- created IAM user
- granted admin acesss to iam user
- generated console access keys
- installed the AWS CLI in gitpod
- turned on billing alerts in billing preferences
- created budget in CLI
- added budget json files via gitpod
- created sns topic in CLI
- confirmed subscription via email
- added alarm json via gitpod

- recreated conceptual diagram on a napkin
![IMG_8023](https://user-images.githubusercontent.com/26096522/219816118-fb4e9974-d619-45ec-be21-164362d0ce84.jpg)

- recreated logical architectural diagram in lucid charts
![Aws Bootcamp](https://user-images.githubusercontent.com/26096522/219816141-1406d9c8-5382-4ea6-a1b1-d52d07983a4e.png)

Problem Areas:
- setting console access keys as env variables in gitpod, setting them was not a problem but I would get an InvalidClientTokenId error upon restarting gitpod
- understanding the architectural diagram components

Solutions:
- standard troubleshooting for the gitpod error
  - update: wokrking, created new keys, deleted all workspaces in gitpod and replaced env vars with new keys, keys work now but "aws sts get-caller-identity" returns id of old keys, checking IAM on aws management console confims new keys are being used and old keys are deactivated.
- research each component in diagram

This weeks takeaways:
- setting up proper security when it comes to IAM on an aws account
  - following the principle of least privilege
- creating IAM users and only using root account for very specific tasks
- setting up cli access to aws account
- setting up budgets and alerts
- how to use lucid charts, an easy to use and very useful tool
