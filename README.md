## Features
Execute change set after review

### **Note**
Use `natluqwerty/create_changeset_and_comment_in_pr@main` to create a changeset

## Prerequisite
Authenticate AWS Account
``` yaml
- name: Authenticate AWS
  uses: aws-actions/configure-aws-credentials@v1
  with:
    role-to-assume: arn:aws:iam::123456789100:role/my-github-actions-role
    role-session-name: Github-Actions-Session
    aws-region: ap-southeast-2
```

## Usage
```yaml
- name: Deploy Changes
  uses: natluqwerty/execute-change-set@main
  with:
    stack-name: your-stack-name
```

## Bug Report
If you find any bug, please let `nat.lu2022@gmail.com` know!! thank you so much!!!! 😃
