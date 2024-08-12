# Enforcing Security Best Practices with AWS SCPs and GCP OPCs

## Overview

 This repository is dedicated to showcasing effective strategies for implementing Organizational Policies (OPCs) and Service Control Policies (SCPs) in cloud environments to achieve a holistic security posture. 

This includes detailed code snippets, configuration files, and real-world use cases to help you secure your cloud infrastructure.

## Repository Structure

- **/policies**: Contains sample Organizational Policies and Service Control Policies.

## Key Features

- **Top 5 Organizational Policies (OPCs)**:
  - Restrict VMs from having external IPs (`compute.vmExternalIpAccess`)
  - Enforce HTTPS communication for GCS (`storage.requireTls`)
  - Disable OS Login for SSH access (`compute.disableOsLogin`)
  - Require Uniform Bucket-Level Access on GCS (`storage.uniformBucketLevelAccess`)
  - Restrict Public IPs for SQL Instances (`sql.restrictPublicIp`)

- **Top 5 Service Control Policies (SCPs)**:
  - Deny Disablement of Security Monitoring (`ec2:DisableVpcClassicLink`)
  - Prevent Deletion of Logging Buckets (`s3:DeleteBucket`)
  - Deny IAM Policies with Wildcards (`iam:PassRole`)
  - Require MFA for IAM Actions (`iam:ChangePassword`)
  - Enforce KMS Key Usage for Encryption (`kms:Decrypt`)

## Value-Add

Implementing these policies enhances your cloud environment's security by reducing exposure to potential threats, ensuring compliance with industry standards, and automating security enforcement across your organization.

## Getting Started

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/cloudsec-best-practices.git
    ```
2. **Navigate to the repository:**
    ```bash
    cd cloudsec-best-practices
    ```
3. **Review the policies:**
    - Browse the `/policies` directory to see the Organizational Policies and Service Control Policies.
4. **Apply the policies:**
    - Use the scripts in `/scripts` to apply the policies in your cloud environment.

## Contribution

We welcome contributions from the community! If you have additional policies, use cases, or enhancements, please feel free to submit a pull request.

## License

This repository is licensed under the MIT License. See `LICENSE` for more information.
