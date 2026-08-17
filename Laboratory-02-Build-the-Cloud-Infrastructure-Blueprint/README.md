# Laboratory 02 - Build the Cloud Infrastructure Blueprint

## Mission Overview
This laboratory focuses on understanding and blueprinting core cloud computing infrastructure by investigating a live Linux server environment and evaluating major public cloud service providers.

## Objectives
- Investigate and document live system configurations and hardware metrics from a cloud-based Linux environment.
- Identify and map essential cloud infrastructure components including compute, storage, networking, and the operating system layer.
- Compare leading public cloud providers (AWS, Microsoft Azure, and Google Cloud Platform) and their equivalent core services.
- Design, visualize, and document a simple, standard-compliant cloud architecture blueprint.

## Cloud Infrastructure Components
- **Compute Resources:** Virtual processing cores responsible for executing instructions and running applications.
- **Storage Resources:** Persistent file systems and disk partitions (such as `/dev/vda1`) used for data management.
- **Networking Resources:** IP addresses and network interfaces that govern communication between servers and external networks.
- **Operating System Layer:** Ubuntu 24.04 LTS, providing the software abstraction layer over physical or virtual hardware.

## Tools Used
- **KillerCoda:** Interactive browser-based Linux environment for server investigation.
- **GitHub:** Version control and repository documentation platform.
- **Diagramming Tool (Canva):** Visual architecture design tool for creating the infrastructure blueprint.

## Linux Commands Executed
- `uname -r` (identifying the kernel version)
- `hostname` (checking system identification)
- `free -h` (monitoring system memory/RAM usage)
- `df -h` (inspecting disk capacity and mounted filesystems)
- `ip a` (viewing network interface configurations and IP addresses)

## Skills Learned
- Correlating low-level operating system parameters with high-level enterprise cloud architecture concepts.
- Differentiating proprietary naming conventions and feature sets across AWS, Azure, and GCP.
- Creating clear, organized technical documentation using standard Markdown.

## Challenges Encountered
- Translating raw terminal metrics into conceptual cloud infrastructure terms.
- Mapping out a clean, logical visual representation of a cloud architecture topology containing user, network, compute, and storage elements.

