# Week 0 — Billing and Architecture

## Required Homework/Tasks

Summary: 
screenshots [assets journal](https://github.com/cloudtrailblaze/aws-bootcamp-cruddur-2023/tree/main/journal/assets)
- Architectural diagrams, conceptual and logical designs 
- Under my pre-existing root account I created a new organization group 
- I created a new IAM user with admin privileges and applied user to new org group 
- Generated AWS credentials / Created access keys for admin user
- Turned on MFA for the IAM user 
- Use Cloudshell 
- Set up budgets and alarms/SNS
- Gitpod configuration (AWS Credentials, AWS CLI)
- Watched video playlist for week0 (thank you Andrew & team 👏)
---


### Install AWS CLI & Verify it's working
---
I admit, intitally I struggled with the installation process but was able to stick with it this is what I did on my local machine: 
1. download the zip file
2. unpacked the zip file
3. installed AWSCLI
4. verified a new instance/workspace would run AWSCLI
5. Commit my changes to Github and verify my work (<em>which included making sure aws keys were set in user-settings on GitPod</em>)

``` curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
$ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```
Once that was completed, I needed to verify the installation would run if I launched my workbook fresh (new) so I closed out of my session and relaunched my workspace as a new instance and then I ran into an error
```invalud gitpod.yml: unparsable Gitpod configuration: YAMLException: end the stream or document separator is expected at line 10, colum 1: vscode:^ ``` After review and backtracking to trace my steps, I had accidently deleted the word tasks: within the command that executes AWSCLI from GitPod on intitial launch. I corrected that mistake and commited the changes, this resolved the issue yay! commit [here](https://github.com/cloudtrailblaze/aws-bootcamp-cruddur-2023/blob/main/.gitpod.yml)


## cli commands for billing and budget alarm
Ran AWSCLI commands for billing and budget alarm and committed my changes to main branch [here](https://github.com/cloudtrailblaze/aws-bootcamp-cruddur-2023/tree/main/aws/json)


## Homework Hard Assignments
Lucid Chart Architectural diagram(s) conceptual and logical :vulcan_salute:
- [Conceptual Napkin attempt:boom:](assets/icloudtrailblaze_conceptual_napkin.jpg)
- [Conceptual Diagram](https://lucid.app/lucidchart/0cd32f9a-eae5-47d8-a249-3e4a551df1e6/view?page=0_0#)
- [Logical Diagram](https://lucid.app/lucidchart/88ea5c3c-8906-4e55-95c8-6b1c676bdbd5/view?page=0_0&invitationId=inv_38cfc8f2-17e8-460b-a4a9-a86628dbf0c9#)
