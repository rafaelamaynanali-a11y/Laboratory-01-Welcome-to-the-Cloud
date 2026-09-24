# Laboratory 03 – Multi-Cloud Explorer

## Mission Overview

This laboratory activity explores Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP). The purpose is to compare their services and identify which platform may fit different business requirements.

## Repository Contents

- `aws-research.md` – research about AWS
- `azure-research.md` – research about Microsoft Azure
- `gcp-research.md` – research about Google Cloud Platform
- `cloud-platform-comparison.md` – comparison of cloud providers and equivalent services
- `client-recommendations.md` – recommendations for four business scenarios and decision matrix
- `reflection.md` – personal reflection about the activity
- `screenshots/` – screenshots used as evidence

## Linux Investigation

The Linux investigation was completed using a KillerCoda playground. The collected information was:

| Item | Result |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS |
| Kernel | 6.8.0-136-generic |
| CPU | Intel Xeon E312xx (Sandy Bridge) |
| CPU Cores | 1 |
| Memory | Approximately 1.9 GiB RAM |
| Disk | Approximately 20 GB |
| Hostname | ubuntu |
| IP Address | 172.30.1.2/24 |
| Network Interface | enp1s0 |

## Possible Cloud Hosting Services

The Linux server could be hosted using the following services:

- **AWS:** Amazon EC2 using an Ubuntu image. Amazon EBS could be used for storage, and Amazon VPC could provide networking.
- **Microsoft Azure:** Azure Virtual Machines using an Ubuntu image. Managed Disks and Azure Virtual Network could support the server.
- **Google Cloud:** Compute Engine using an Ubuntu image. Persistent Disk and Virtual Private Cloud networking could be used.

The exact machine size should be selected according to the server's workload, memory needs, storage requirements, security, and budget.

## Evidence

The `screenshots` folder contains the homepage screenshots for the three cloud providers, the KillerCoda terminal screenshot, and the GitHub repository screenshot.

## Sources

- [AWS Documentation](https://docs.aws.amazon.com/)
- [Microsoft Azure Documentation](https://learn.microsoft.com/azure/)
- [Google Cloud Documentation](https://cloud.google.com/docs)
