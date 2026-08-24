# Laboratory Activity 3: Multi-Cloud Explorer

## Checkpoint 7 – Linux Server Investigation & Cloud Migration

### 1. Linux System Investigation Results
By running diagnostic commands in the KillerCoda playground terminal, the system details were identified as follows:
* **Operating System:** Ubuntu (identified via `cat /etc/os-release`)
* **CPU Information:** Intel/AMD virtualized processor details (identified via `lscpu`)
* **Memory:** Total RAM and available swap allocation (identified via `free -h`)
* **Disk Space:** Total storage capacity and partition usage (identified via `df -h`)

### 2. Cloud Migration Recommendations
If this Linux server were to be migrated to the cloud, it can be hosted using the core virtual machine services of the major cloud providers:

* **Amazon Web Services (AWS):** 
  * **Service:** Amazon Elastic Compute Cloud (Amazon EC2)
  * **Details:** Provides secure, resizable compute capacity in the cloud using customizable Amazon Machine Images (AMIs) running Linux.
* **Microsoft Azure:** 
  * **Service:** Azure Virtual Machines
  * **Details:** Offers on-demand, scalable Linux virtual machine instances with flexible sizing and management tools.
* **Google Cloud Platform (GCP):** 
  * **Service:** Google Compute Engine (GCE)
  * **Details:** Allows you to create and run virtual machines on Google's innovative infrastructure, supporting custom machine types and fast booting.

---
*Screenshots of the terminal commands and outputs have been saved to `screenshots/killercoda-terminal.png`.*
