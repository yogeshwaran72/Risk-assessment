# Risk-assessment

## Aim:
To perform an asset-oriented risk assessment of cloud storage assets including:
● AWS Elastic Block Store (EBS)
● AWS Elastic File System (EFS)
● Azure Files (File Storage)

## Pre-requisites:
# 1.Background:
Cloud storage services offer flexible, scalable options for storing data. However, each storage type
brings distinct security risks and configurations. This experiment focuses on identifying assets and
performing a detailed risk assessment based on confidentiality, integrity, and availability (CIA), access
control, encryption, and auditing capabilities.

# 2.Tools Required:
● AWS Console with EC2, EBS, and EFS access
● Azure Portal with Storage Account access
● IAM credentials with sufficient permissions
● Risk Assessment Template (provided)
● Internet browser
● Microsoft Excel or Google Sheets for  tabulating findings

## 4. Procedure:
Part A: Identifying AWS Storage Assets
Step 1: Login to AWS Console
● Go to https://aws.amazon.com/console
● Log in using IAM or root credentials

Step 2: Identify EBS Volumes
● Navigate to EC2 > Volumes (under Elastic Block Store)
● Observe and record the following for each volume:
● Volume ID
● Size and Type (e.g., gp2, io1)
● Availability Zone
● Attached instance (if any)
● Encryption status
● Tags

Step 3: Identify EFS File Systems
● Go to EFS > File systems
● For each file system, record:
● File system ID and name
● Mount targets (AZs)
● Throughput mode (bursting/provisioned)
● Performance mode
● Lifecycle policy
● Encryption at rest status
Part B: Identifying Azure File Storage Assets

Step 4: Login to Azure Portal
● Go to https://portal.azure.com
● Log in using credentials with access to storage accounts

Step 5: View File Shares
● Navigate to Storage Accounts > Choose Account > File Shares
● For each file share, record:
● Name
● Quota (in GB)
● Used space
● Protocol (SMB/NFS)
● Authentication method (SAS Tokens, Azure AD, Shared Keys)
● Snapshot policies

## 5. Risk Assessment Methodology
Use the following CIA-based asset-oriented checklist for each asset:
![image](https://github.com/user-attachments/assets/fcdb9674-6c2b-4812-8275-b24a9d39e1e2)


## Sample Output:
![image](https://github.com/user-attachments/assets/c2163265-c8eb-4742-9520-074dd61d8972)


## 6. Observations and Tabulation
Cloud
Provider
Asset Type Asset ID Encrypted Access Control Risk Level Comments
AWS EBS Volume vol-abc Yes IAM Policy Medium Used by EC2
AWS EFS fs-xyz Yes Security Group Low Multi-AZ mount
Azure File Share datafiles Yes Shared Key Medium Quota 1TB

## Result:
You have identified all active storage assets and evaluated them based on security posture and risk level.
