# Cloud Infrastructure Components - KillerCoda Environment

## 1. Compute Resources
- **Description:** Virtual CPU cores and processing power allocated to the instance.
- **KillerCoda Context:** Managed via the Linux kernel, utilizing virtual processing power to execute instructions and run background services.
- **Cloud Importance:** Essential for running applications, processing workloads, and handling user requests dynamically.

## 2. Storage Resources
- **Description:** Disk capacity and file systems used to store data, configurations, and applications.
- **KillerCoda Context:** The root file system (`/dev/vda1` with 19G capacity), along with `/boot` and `/boot/efi` partitions.
- **Cloud Importance:** Provides persistent and temporary data storage required for operating systems and application state management.

## 3. Networking Resources
- **Description:** IP addresses and network interfaces enabling communication between the server and external networks.
- **KillerCoda Context:** The assigned container/VM IP addresses (`172.30.1.2`, `172.17.0.1`) and loopback interfaces.
- **Cloud Importance:** Allows services to communicate securely, accept incoming web traffic, and connect to other distributed cloud components.

## 4. Operating System Layer
- **Description:** The system software that manages hardware resources and provides common services for programs.
- **KillerCoda Context:** Ubuntu 24.04 LTS environment.
- **Cloud Importance:** Acts as the bridge between the raw infrastructure hardware and the deployed cloud applications.
